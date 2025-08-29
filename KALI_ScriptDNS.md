### Criando arquivos com dados dentro e mostrando os dados dentro

```txt
vi teste1.txt

www

vi teste2.txt

mail

vi teste3.txt

ftp

cat teste1.txt
cat teste2.txt
cat teste3.txt

```

### Concatenando arquivos com CAT

```txt

vi dominios1.lst

cat teste1.txt teste2.txt teste3.txt > dominios1.lst

```

### Linha do tempo de comandos que utilizei

```txt
┌──(laboratorio㉿lab24dt01)-[/home]
└─$ cd laboratorio
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ ls -la
total 120
drwx------ 16 laboratorio laboratorio  4096 ago 29 08:02  .
drwxr-xr-x  3 root        root         4096 out 15  2024  ..
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024 'Área de trabalho'
-rw-r--r--  1 laboratorio laboratorio   220 out 15  2024  .bash_logout
-rw-r--r--  1 laboratorio laboratorio  5551 out 15  2024  .bashrc
-rw-r--r--  1 laboratorio laboratorio  3526 out 15  2024  .bashrc.original
drwxrwxr-x  2 laboratorio laboratorio  4096 ago 29 07:54  .bully
drwx------ 13 laboratorio laboratorio  4096 out 15  2024  .cache
drwxr-xr-x 17 laboratorio laboratorio  4096 ago 18 19:42  .config
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Documentos
-rw-rw-r--  1 laboratorio laboratorio    40 ago 22 10:51  dominios.lst
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Downloads
-rw-r--r--  1 laboratorio laboratorio 11759 out 15  2024  .face
lrwxrwxrwx  1 laboratorio laboratorio     5 out 15  2024  .face.icon -> .face
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Imagens
drwxr-xr-x  3 laboratorio laboratorio  4096 out 15  2024  .java
drwxr-xr-x  4 laboratorio laboratorio  4096 out 15  2024  .local
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Modelos
drwx------  4 laboratorio laboratorio  4096 out 15  2024  .mozilla
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Músicas
-rw-r--r--  1 laboratorio laboratorio   807 out 15  2024  .profile
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Público
-rw-r--r--  1 laboratorio laboratorio     0 out 15  2024  .sudo_as_admin_successful
drwxr-xr-x  2 laboratorio laboratorio  4096 out 15  2024  Vídeos
-rw-------  1 laboratorio laboratorio   825 ago 22 10:55  .viminfo
-rw-------  1 laboratorio laboratorio   799 ago 29 07:54  .zsh_history
-rw-r--r--  1 laboratorio laboratorio 10868 out 15  2024  .zshrc
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ pwd
/home/laboratorio
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste1.txt  

[Alterações não gravadas]

Aperte ENTER ou digite um comando para continuar
[Alterações não gravadas]

Aperte ENTER ou digite um comando para continuar
[Alterações não gravadas]

Aperte ENTER ou digite um comando para continuar
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi                       


Aperte ENTER ou digite um comando para continuar
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste1.txt
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste1.txt
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat teste1.txt  
www
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste2.txt
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat teste2.txt
mail
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste3.txt 
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste3.txt
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi teste3.txt 
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat dominios.lst
google.com
uol.com.br
clubedores.com.br
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat teste1.txt teste2.txt teste3.txt > dominios.lst
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat dominios.lst                                   
www
mail
ftp
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi dominios1.lst
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi              
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ vi dominios1.lst
                                                                                                                                                                                                                                              
┌──(laboratorio㉿lab24dt01)-[~]
└─$ cat dominios1.lst
www
mail
ftp


```

# 📘 Explicação do script `busca_subdominios.sh`

## O que o script faz
Ele lê uma lista de **prefixos de subdomínio** (ex.: `www`, `mail`, `ftp`) do arquivo `dominios1.lst` e, para **cada** prefixo, consulta o DNS para saber se o **subdomínio existe** para um **domínio** que você passa como parâmetro na execução (ex.: `google.com`).  
Só mostra as linhas que realmente resolvem para um **endereço IPv4**.

---

## Script
```bash
#!/bin/bash
for url in $(cat dominios1.lst)
do host $url.$1 | grep "has address"
done
```

## (Opcional) Versão mais robusta
```bash
#!/bin/bash
while IFS= read -r url; do
  host "$url.$1" | grep "has address"
done < dominios1.lst
```
---

## Explicação linha por linha

### 1) Shebang
```bash
#!/bin/bash
```
- Diz ao sistema: “execute este arquivo usando o **bash**”.

---

### 2) Laço `for`
```bash
for url in $(cat dominios1.lst)
```
- Lê cada linha de `dominios1.lst` e guarda em `url`.  
- Exemplo do arquivo:
  ```
  www
  mail
  ftp
  ```

---

### 3) Consulta DNS
```bash
do host $url.$1 | grep "has address"
```
- Monta `subdominio.dominio` (`www.google.com`).  
- `host` consulta o DNS.  
- `grep "has address"` filtra apenas os endereços IPv4 (registro **A**).

---

### 4) Fim do laço
```bash
done
```
- Finaliza o laço `for`.

---

## Como usar

### Criar lista de subdomínios
```txt
dominios1.lst
-------------
www
mail
ftp
```

### Dar permissão de execução
```bash
chmod a+x busca_subdominios.sh
```

### Executar
```bash
./busca_subdominios.sh ufn.edu.br
```

---

## 🔑 Comandos de Permissões (chmod)

### Representação numérica
- **1 → Executar**  
- **2 → Gravar**  
- **4 → Ler**

As permissões são somadas.  
Exemplo:
- `7` = 4 (ler) + 2 (gravar) + 1 (executar).  
- `6` = 4 (ler) + 2 (gravar).  
- `5` = 4 (ler) + 1 (executar).  

### Estrutura
São **três blocos**:  
```
Owner (dono) | Grupo | Outros
```

### Exemplos que você executou
- `chmod a+x busca_subdominios.sh` → deu execução para **todos**.  
- `chmod a-x busca_subdominios.sh` → removeu execução de **todos**.  
- `chmod 111 busca_subdominios.sh` → só executável, sem leitura ou escrita.

---

## 🌐 Por que aparecem IPs diferentes?

### Exemplo
```bash
./busca_subdominios.sh ufn.edu.br
# Resultado:
www.ufn.edu.br has address 200.132.59.110

./busca_subdominios.sh host ufn.edu.br
# Resultado:
mail.host has address 52.20.84.62
```

### Explicação
- O **DNS** é como uma "agenda telefônica" da internet.  
- Cada subdomínio pode apontar para **servidores diferentes**, que cumprem funções distintas:
  - `www.ufn.edu.br` → aponta para o **servidor web da UFN** (IP brasileiro: 200.132.59.110).  
  - `mail.host` → aponta para um **servidor de e-mail**, que muitas vezes está em outro provedor (nesse caso, IP da AWS: 52.20.84.62).  

### Motivos para IPs diferentes
1. **Funções distintas**: um IP para web, outro para e-mail, outro para FTP etc.  
2. **Infraestrutura distribuída**: universidades/empresas usam serviços externos (como AWS, Google, Microsoft) para e-mail.  
3. **Localização**: IP local (Brasil) pode ser para site, IP internacional para serviços terceirizados.

👉 Isso é **normal** e até recomendado para dividir carga e segurança.  

---

## Observação sobre IPs

- Um **mesmo domínio** pode ter **múltiplos IPs**, dependendo dos serviços.  
- Isso acontece porque empresas geralmente **separam serviços críticos** (site, e-mail, painel, etc.) em servidores distintos.  
- Assim, se um servidor cair, os outros continuam funcionando.

Exemplo prático:
- `www.ufn.edu.br` → 200.132.59.110 (servidor web da universidade)  
- `mail.ufn.edu.br` → 52.20.84.62 (servidor de e-mail hospedado na Amazon AWS)


---
---

# Revisão 

### Comandos de Permissões

1 - Permite executar
2 - Permite gravar
3 - Permite leitura

Exemplo:

1 1 1

Representa permissões para:

Owner (Dono) | Grupo (Group) | Outros (Outros)


# Diferença entre Subdomínios Comuns

Cada subdomínio representa **um serviço diferente** hospedado dentro do mesmo domínio principal.  
Eles podem ou não compartilhar o mesmo **endereço IP**, dependendo da infraestrutura do servidor.

## Subdomínios mais comuns:

- **www** → Geralmente aponta para o **site principal**.  
  - Impacto no IP: Pode ser o mesmo IP do domínio raiz ou um servidor dedicado para web.

- **mail** → Usado para serviços de **e-mail** (SMTP, IMAP, POP3, webmail).  
  - Impacto no IP: Normalmente aponta para o servidor de e-mail, que pode estar em outro provedor (ex: Google, Microsoft).

- **ftp** → Usado para o protocolo **FTP** (File Transfer Protocol), para envio/recebimento de arquivos.  
  - Impacto no IP: Pode ser o mesmo do site ou um servidor exclusivo de arquivos.

- **docs** → Usado para hospedar **documentação** ou arquivos compartilhados (ex: Google Docs em empresas).  
  - Impacto no IP: Muitas vezes é um servidor ou serviço separado.

- **tribo** → Subdomínio personalizado, pode ser um **portal interno, fórum ou comunidade**.  
  - Impacto no IP: Vai depender de onde está hospedado, geralmente separado.

- **painel** → Usado para **acesso administrativo** (ex: painel de hospedagem, painel de cliente, cPanel, Plesk).  
  - Impacto no IP: Pode estar no mesmo servidor do site, mas muitas vezes é separado por questões de segurança.

---







