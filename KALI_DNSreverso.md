# 🔎 DNS Reverso e Script em Bash

## 📌 O que é DNS Reverso?
O **DNS reverso** é o processo de consultar o nome associado a um endereço IP.  
Enquanto o DNS normal resolve **nomes → IPs** (exemplo: `www.ufn.edu.br` → `200.132.59.110`),  
o **DNS reverso** faz o caminho contrário: **IPs → nomes**.

Isso é feito através de registros **PTR** no DNS.

- Se um IP tem registro PTR → você verá um **nome de host** associado.  
- Se não tem registro PTR → o retorno será algo como `NXDOMAIN` (não existe domínio associado).

Exemplo prático:

```bash
host 200.132.59.110
# 110.59.132.200.in-addr.arpa domain name pointer www.ufn.edu.br.
```

Aqui, o IP `200.132.59.110` está associado ao nome `www.ufn.edu.br`.

---

## 📜 Script para Consulta de DNS Reverso

Aqui está um script simples em **Bash** que faz uma varredura de IPs e tenta resolver seus nomes via DNS reverso:

```bash
#!/bin/bash
for ip in $(seq 0 255);
do 
    host $1.$ip
done
```

### 🔎 Explicação linha por linha:
1. `#!/bin/bash` → Define que o script será executado no interpretador **Bash**.  
2. `for ip in $(seq 0 255);` → Cria um laço que percorre os números de `0 a 255`.  
   - Isso corresponde à última parte de um endereço IPv4 (ex.: `200.132.144.X`).  
3. `do host $1.$ip` → Executa o comando **host** para cada IP, usando como base o valor passado no parâmetro `$1`.  
   - Exemplo: se você rodar `./dns_reverso.sh 200.132.144`, o script vai testar `200.132.144.0`, `200.132.144.1`, ..., `200.132.144.255`.  
4. `done` → Finaliza o loop.

---

## ▶️ Como Executar

1. Salve o script em um arquivo chamado `dns_reverso.sh`.  
2. Dê permissão de execução:  
   ```bash
   chmod +x dns_reverso.sh
   ```
3. Execute passando a **base do IP** (os 3 primeiros blocos):  
   ```bash
   ./dns_reverso.sh 200.132.144
   ```

Se houver algum IP nessa faixa com **registro PTR configurado**, o script mostrará o domínio associado.  
Se não houver, você verá mensagens de erro como:  
`Host 200.132.144.X not found: 3(NXDOMAIN)`.

---

## ✅ Resumindo
- **DNS normal:** nome → IP.  
- **DNS reverso:** IP → nome (via registro PTR).  
- O script automatiza a consulta de uma faixa de IPs.  
