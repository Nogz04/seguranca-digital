**Enunciado da Questão - Resposta dela abaixo.**

**Questão 1 - O que é engenharia Social? Dê um exemplo.**

Engenharia Social é um tipo de ataque que explora as vulnerabilidades humanas, como o desejo de ser prestativo e a falta de conscientização sobre políticas de segurança, em vez de explorar falhas em sistemas. O objetivo é convencer um funcionário ou usuário a fornecer informações sensíveis da empresa, o que pode anular outros controles de segurança existentes.

Um exemplo famoso é o do hacker Kevin Mitnick, que conseguiu acesso a um prédio simplesmente convencendo o segurança de que ele tinha permissão para estar no local. Outro exemplo seria um atacante ligar para o suporte de TI (help desk) de uma empresa, fingindo ser um funcionário em apuros que não consegue acessar sua conta, para induzir o atendente a resetar ou fornecer uma senha.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 2 - Descreva o processo de uma conexão TCP.**

O processo de estabelecimento de uma conexão TCP (Protocolo de Controle de Transmissão) é conhecido como **"Three-Way Handshake"** (Aperto de Mão de Três Vias). Ele garante que ambos os dispositivos, cliente e servidor, estejam prontos para a comunicação e sincronizados. O processo ocorre em três etapas:

1.  **SYN:** O cliente que deseja iniciar a comunicação envia um pacote de dados com a flag `SYN` (de *synchronize*) para o servidor. Este pacote informa ao servidor que o cliente deseja estabelecer uma conexão e qual é o seu número de sequência inicial.
2.  **SYN-ACK:** Ao receber o pacote `SYN`, o servidor responde com um pacote que possui as flags `SYN` e `ACK` (de *acknowledgment*). Com isso, o servidor confirma o recebimento do pedido do cliente (`ACK`) e também envia seu próprio número de sequência inicial (`SYN`), indicando que está pronto para se conectar.
3.  **ACK:** Por fim, o cliente recebe o pacote `SYN-ACK` do servidor e envia um último pacote, contendo apenas a flag `ACK`. Este pacote confirma que o cliente recebeu a resposta do servidor.

Após a conclusão dessas três etapas, a conexão TCP é considerada estabelecida, e a transferência de dados entre o cliente e o servidor pode começar.

Sobre uso em invasões, a comunicação TCP pode ser abusada, por exemplo, para varredura de portas (port scanning), onde atacantes enviam pacotes SYN para descobrir quais portas estão abertas e, assim, identificar serviços vulneráveis. Também pode ser usada em ataques como SYN Flood, que tenta sobrecarregar o servidor enviando muitas solicitações iniciais (SYN) sem completar a conexão, causando indisponibilidade.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 3 - O que é Deepfake?**

Deepfake é uma tecnologia de inteligência artificial usada para criar vídeos ou áudios falsos, porém realistas, com o objetivo de se passar por outra pessoa. Essa tecnologia pode ser utilizada por fraudadores para enganar funcionários e cometer crimes.

Um exemplo citado foi o de um funcionário do setor financeiro de uma multinacional que foi enganado para transferir 25 milhões de dólares a golpistas. Os criminosos usaram a tecnologia deepfake para se passar pelo diretor financeiro da empresa durante uma chamada de vídeo, fazendo com que a transação parecesse legítima.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 4 - O que significa DDNS e como ele funciona? Pode dar um exemplo para explicar.**

DDNS significa *Dynamic DNS* (DNS Dinâmico). Ele é um método utilizado para atualizar automaticamente um servidor de nomes (DNS) quando o endereço IP associado a um nome de domínio não é fixo, mas sim dinâmico, como os fornecidos por muitos provedores de internet. O DDNS funciona ativando nomes de hosts, endereços ou outras informações configuradas para que um dispositivo possa ser acessado remotamente mesmo que seu endereço IP mude.

Um exemplo de sua utilização é para acessar equipamentos IP remotamente, como câmeras de segurança, babás eletrônicas ou para o funcionamento de softwares como o TeamViewer, que precisam de uma conexão estável a um dispositivo cujo endereço IP pode variar.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 5 - Qual a diferença entre Phreakers e Defacers?**

A principal diferença entre Phreakers e Defacers está no alvo e no objetivo de suas ações:

* **Phreakers:** O objetivo de um phreaker é quebrar a segurança de sistemas de telefonia, seja fixa ou móvel, com a intenção de utilizar os serviços gratuitamente. Suas técnicas envolvem a exploração de falhas para, por exemplo, clonar aparelhos e realizar ligações sem custo.
* **Defacers:** Também conhecidos como "pichadores virtuais", o objetivo dos defacers é alterar a aparência de uma ou mais páginas de um site. Eles invadem o servidor para modificar o conteúdo, geralmente deixando mensagens de protesto, com ideais políticos ou simplesmente para mostrar que o site estava vulnerável.

Em resumo, phreakers focam em sistemas de telefonia para obter serviços gratuitos, enquanto defacers focam em desfigurar visualmente páginas da web.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 6 - Explique o que é zona de DNS e por que ocorre a sua transferência?**

Uma zona de DNS é uma parte do banco de dados do DNS que contém os registros responsáveis por um domínio ou subdomínio específico (como A, MX, CNAME, etc.).
A transferência de zona ocorre para que servidores DNS secundários recebam uma cópia atualizada dessa zona, garantindo redundância, disponibilidade e consistência das informações de resolução de nomes.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 7 - Como funciona o Algoritmo PageRank?**

O PageRank é um algoritmo da Google que mede a importância de um site com base nos links mencionados desse site em outros sites do page rank, assim, mostrando sua importância.

Links mencionados =  (cliques no link que leva para o site, quantidade de links desse site presentes em outros sites, etc...) 

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 8 - Quando e onde surgiu o termo Hacker?**

O termo "Hacker" surgiu pela primeira vez em 1950, no MIT (Massachusetts Institute of Technology) no Jargão da Informática. Originalmente, ele era usado para designar indivíduos interessados na ciência do Processamento Eletrônico de Dados e que se engajavam em alterar algo já existente com o intuito de aperfeiçoá-lo.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 9 - Como podemos verificar quais os servidores de DNS que o nosso sistema operacional Linux está utilizando?**

Em um sistema operacional como o Kali Linux, as configurações dos servidores de DNS podem ser verificadas no arquivo `resolv.conf`, que está localizado no diretório `/etc`. Para visualizar o conteúdo deste arquivo e, consequentemente, os servidores de DNS (identificados como `nameserver`), pode-se utilizar o comando `cat /etc/resolv.conf` no terminal.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 10 - O que garante que o trabalho de um Hacker ético, não seja considerado crime?**

O que garante que o trabalho de um hacker ético não seja considerado crime é a existência de um contrato devidamente assinado por ambas as partes (o profissional e a empresa contratante). Esse documento autoriza a execução do teste de invasão, especificando o escopo e os limites da atuação. Dessa forma, o contrato serve como uma proteção legal que evita possíveis processos judiciais ou imputações de culpa.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 11 - Quando o servidor secundário de DNS é acionado?**

O servidor secundário de DNS é acionado principalmente em duas situações:

1.  Quando o servidor primário (master) para de funcionar por algum motivo, o servidor secundário, que é uma cópia dele, passa a ser utilizado pelos clientes para resolver as consultas de nomes.
2.  Quando um servidor DNS primário está com sua lista de domínios desatualizada e não consegue responder a uma solicitação, ele passa a consulta para o servidor secundário na tentativa de obter uma resposta.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 12 - O que esta consulta irá retornar, de acordo com o Google Hacking? Site:com.br filetype:txt intext:senhas.**

Esta consulta, utilizando técnicas de **Google Hacking** (também conhecido como Google Dorking), irá retornar uma lista de resultados de pesquisa que atendem a três critérios específicos e combinados:

1.  **`site:com.br`**: Restringe a busca apenas para páginas e arquivos localizados em domínios brasileiros, que terminam com `.com.br`.
2.  **`filetype:txt`**: Filtra os resultados para mostrar apenas arquivos de texto puro, com a extensão `.txt`.
3.  **`intext:senhas`**: Procura pela palavra exata "senhas" dentro do conteúdo (corpo do texto) desses arquivos.

Portanto, o resultado final será uma lista de arquivos de texto (`.txt`) hospedados em sites brasileiros (`.com.br`) que contêm a palavra "senhas" em seu conteúdo. Este tipo de busca é frequentemente usado por pesquisadores de segurança (e atacantes) para encontrar informações sensíveis, como listas de usuários e senhas, que foram acidentalmente expostas e indexadas publicamente na internet.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 13 - O que é um Malware?**

É um arquivo malicioso que tem como objetivo invadir/prejudicar o sistema/máquina (PC ou Mobile) do usuário. Ex: Cavalo de Tróia

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 14 - O que é um exploit?**

Um exploit é um programa ou código que se aproveita de uma
falha de segurança (vulnerabilidade) em um sistema, software
ou hardware para executar comandos não autorizados. 

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 15 - O que é Metasploit?**

O Metasploit é uma ferramenta de segurança usada para testes de penetração. Ele reúne exploits, payloads e módulos que permitem avaliar vulnerabilidades de sistemas de forma controlada, ajudando profissionais de segurança a identificar falhas e verificar se proteções estão funcionando.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 16 - O que é Payload?**

Um payload é o código que executa a ação final após uma vulnerabilidade ser explorada. Ele pode ser usado de forma maliciosa ou em testes de segurança autorizados.
O payload define o que será feito no sistema comprometido, como o tipo de conexão que será estabelecida, quais comandos poderão ser executados e qual nível de acesso será obtido.


***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 17 -  Explique o que é o PayLoad windows/meterpreter/reverse_tcp?**


Ele é um Payload feito para invadir windows após a exploração de uma vulnerabilidade, esse Payload tem como objetivo conseguir uma sessão Meterpreter na máquina da vítima utilizando um metódo de conexão chamado reverse_tcp, o reverse_tcp funciona da seguinte maneira:

Esse Payload faz com que a conexão parta de dentro da máquina da vítima até a máquina do Hacker (de dentro para fora), ou seja, o Payload vai até a porta da vítima (no IP tal e porta TAL), a máquina lê as instruções do Payload que diz: "Venha até a minha máquina (do Hacker), IP -> 192.168.?.?, Porta -> 4444, e se conecte a mim", com isso, a porta 4444 do Hacker vai ficar esperando a vítima vir, quando ela vir, a conexão será estabelecida entre o Hacker e a vítima e o Hacker terá uma sessão Meterpreter.

***

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 18 -  Explique o que é o adobe_pdf_embedded_exe**



No Metasploit, o módulo adobe_pdf_embedded_exe é um exploit que cria um arquivo PDF especialmente modificado, no qual é possível embutir (embed) um executável dentro do documento.
Esse módulo era usado em testes de segurança para demonstrar como PDFs antigos do Adobe Reader podiam ser manipulados para executar código (Payload) no computador da vítima caso ela abrisse o arquivo, assim estabelecendo uma conexão entre a Vítima e o Hacker.

Variáveis:

```msf

INFILENAME: É o PDF de entrada que será modificado. Indica qual arquivo PDF original será usado como base. O módulo pega esse PDF e injeta nele o conteúdo adicional malicioso.

FILENAME: É o nome do arquivo PDF de saída. É o nome do PDF final que será gerado após a modificação (injeção do conteúdo adicional malicioso).

OUTPUTPATH: Define a pasta onde o PDF gerado será salvo.

LHOST: IP do Invasor
LPORT: Porta do Invasor

SET PAYLOAD windows/meterpreter/reverse_tcp
```

**Enunciado da Questão - Resposta dela abaixo.**

**Questão 19 -  Cite três formas de descobrir o servidor de DNS de um serviço hospedado na WWW:**

WhoIs
nslookup (nslookup -type=NS dominio.com)
dig (dig NS dominio.com)

# Variáveis para setar nos exploits:

LHOST: IP do Invasor 

LPORT: Porta do Invasor

RHOST: IP da Vítima

RPORT: Porta da Vítima

PAYLOAD : Payload para invasão

# Como setar? 

SET LHOST 192.168.?.?
SET LPORT 4444
SET PAYLOAD windows/meterpreter/reverse_tcp
