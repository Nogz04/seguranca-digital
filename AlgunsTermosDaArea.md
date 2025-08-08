# Siglas e Significados - Redes, Comunicação de Dados e Segurança Digital

---

## 💻 Redes de Computadores

### IP - Internet Protocol

**Significado:** Protocolo de Internet  
📌 O IP é o protocolo responsável por endereçar e encaminhar pacotes de dados entre dispositivos em redes, como a internet.  
🔍 Cada dispositivo em uma rede IP possui um endereço IP único. Existem duas versões: IPv4 (ex: 192.168.0.1) e IPv6 (ex: 2001:db8::1).

---

### TCP - Transmission Control Protocol

**Significado:** Protocolo de Controle de Transmissão  
📌 Protocolo de transporte confiável que garante a entrega correta de dados entre dispositivos. Usa confirmações e retransmissões.  
🔍 Utilizado em serviços como HTTP, e-mail e FTP, onde a integridade dos dados é essencial.

---

### UDP - User Datagram Protocol

**Significado:** Protocolo de Datagrama de Usuário  
📌 Protocolo de transporte sem conexão e mais rápido que o TCP, porém sem garantia de entrega.  
🔍 Usado em aplicações que priorizam velocidade, como streaming de vídeo, chamadas VoIP e jogos online.

---

### MAC - Media Access Control

**Significado:** Controle de Acesso ao Meio  
📌 Endereço físico único atribuído a interfaces de rede, como placas Ethernet e Wi-Fi. Opera na camada 2 do modelo OSI.  
🔍 Identifica dispositivos dentro de uma rede local (LAN), sendo essencial em switches e ARP.

---

### LAN - Local Area Network

**Significado:** Rede de Área Local  
📌 Rede restrita geograficamente, como em casas, escolas ou empresas. Costuma ter alta velocidade e baixa latência.  
🔍 Conecta computadores e dispositivos dentro de um mesmo ambiente físico.

---

### WAN - Wide Area Network

**Significado:** Rede de Área Ampla  
📌 Rede que cobre grandes áreas geográficas, como cidades, países ou continentes.  
🔍 A internet é o maior exemplo de WAN. ISPs usam WANs para conectar clientes.

---

### WLAN - Wireless Local Area Network

**Significado:** Rede de Área Local Sem Fio  
📌 É uma LAN que utiliza comunicação via ondas de rádio (Wi-Fi) ao invés de cabos.  
🔍 Comum em casas, escritórios e locais públicos com roteadores Wi-Fi.

---

### VPN - Virtual Private Network

**Significado:** Rede Privada Virtual  
📌 Cria uma conexão segura e criptografada sobre uma rede pública, como a internet.  
🔍 Usada para acessar redes corporativas remotamente ou proteger a navegação pública.

---

### NAT - Network Address Translation

**Significado:** Tradução de Endereço de Rede  
📌 Técnica que permite múltiplos dispositivos em uma rede privada compartilharem um único endereço IP público.  
🔍 Utilizado em roteadores domésticos para conectar diversos dispositivos à internet.

---

### DNS - Domain Name System

**Significado:** Sistema de Nomes de Domínio  
📌 Converte nomes de sites (como google.com) em endereços IP que computadores usam para se comunicar.  
🔍 Essencial para a navegação na internet — sem DNS, você teria que lembrar IPs numéricos.

---

### DHCP - Dynamic Host Configuration Protocol

**Significado:** Protocolo de Configuração Dinâmica de Host  
📌 Protocolo que atribui automaticamente endereços IP e outras configurações de rede aos dispositivos.  
🔍 Usado por roteadores para configurar computadores, smartphones e impressoras automaticamente.

---

### ISP - Internet Service Provider

**Significado:** Provedor de Serviços de Internet  
📌 Empresa que fornece acesso à internet a usuários e organizações.  
🔍 Exemplos: Claro, Vivo, Oi, Tim, etc.

---

### TTL - Time To Live

**Significado:** Tempo de Vida  
📌 Valor que limita o tempo (ou número de saltos) que um pacote de dados pode permanecer na rede antes de ser descartado.  
🔍 Ajuda a evitar que pacotes fiquem presos em loops na rede.

---

### ARP - Address Resolution Protocol

**Significado:** Protocolo de Resolução de Endereço  
📌 Converte endereços IP em endereços MAC dentro de uma LAN.  
🔍 Fundamental para que computadores saibam para qual hardware local enviar os dados.

---

### ICMP - Internet Control Message Protocol

**Significado:** Protocolo de Mensagens de Controle da Internet  
📌 Usado para enviar mensagens de erro e diagnóstico entre dispositivos de rede.  
🔍 Utilizado em comandos como `ping` e `traceroute` para testar conectividade e rota.

## 📡 Comunicação de Dados

### OSI - Open Systems Interconnection

**Significado:** Interconexão de Sistemas Abertos  
📌 Modelo teórico criado pela ISO que padroniza como os dispositivos se comunicam em uma rede. Divide a comunicação em 7 camadas: Física, Enlace, Rede, Transporte, Sessão, Apresentação e Aplicação.  
🔍 Usado como referência para desenvolvimento de protocolos e equipamentos de rede, facilitando a interoperabilidade entre sistemas diferentes.

---

### ISO - International Organization for Standardization

**Significado:** Organização Internacional de Padronização  
📌 Entidade que desenvolve normas internacionais em diversas áreas, incluindo tecnologia da informação e comunicação.  
🔍 Criadora do modelo OSI e de muitos outros padrões que garantem compatibilidade entre sistemas e segurança digital.

---

### IEEE - Institute of Electrical and Electronics Engineers

**Significado:** Instituto de Engenheiros Eletricistas e Eletrônicos  
📌 Organização profissional global que define padrões técnicos, como o IEEE 802.3 (Ethernet) e IEEE 802.11 (Wi-Fi).  
🔍 Seus padrões são amplamente adotados na indústria de redes e comunicação.

---

### QoS - Quality of Service

**Significado:** Qualidade de Serviço  
📌 Conjunto de técnicas para gerenciar o tráfego da rede, priorizando determinados tipos de dados (como voz ou vídeo) para garantir desempenho.  
🔍 Essencial em redes com múltiplos tipos de tráfego — por exemplo, priorizando chamadas VoIP em uma empresa.

---

### FTTH - Fiber To The Home

**Significado:** Fibra até a Residência  
📌 Tecnologia que entrega internet de alta velocidade via fibra óptica diretamente na casa do usuário.  
🔍 Oferece maior estabilidade e velocidade que tecnologias como ADSL ou cabo coaxial.

---

### DSL - Digital Subscriber Line

**Significado:** Linha Digital de Assinante  
📌 Transmite dados digitais por linhas telefônicas convencionais. Existem variações como ADSL e VDSL.  
🔍 Foi uma das primeiras formas de internet banda larga residencial, hoje sendo substituída por fibra.

---

### PSTN - Public Switched Telephone Network

**Significado:** Rede Telefônica Pública Comutada  
📌 Rede tradicional de telefonia fixa usada para fazer chamadas comutada por circuitos.  
🔍 Base para o funcionamento de linhas telefônicas residenciais e comerciais.

---

### TDM - Time Division Multiplexing

**Significado:** Multiplexação por Divisão de Tempo  
📌 Técnica de transmissão onde vários sinais compartilham o mesmo meio físico, sendo enviados em diferentes intervalos de tempo.  
🔍 Usado em redes digitais, como sistemas telefônicos e comunicação via satélite.

---

### FDM - Frequency Division Multiplexing

**Significado:** Multiplexação por Divisão de Frequência  
📌 Técnica onde múltiplos sinais são transmitidos simultaneamente usando diferentes frequências em um único canal.  
🔍 Utilizado em transmissões de rádio, TV a cabo e comunicação analógica.

---

### BPS - Bits Per Second

**Significado:** Bits por Segundo  
📌 Unidade de medida da taxa de transmissão de dados.  
🔍 Utilizada para medir a velocidade de links de rede, como “100 Mbps” ou “1 Gbps”.

---

### BER - Bit Error Rate

**Significado:** Taxa de Erro de Bits  
📌 Proporção entre a quantidade de bits transmitidos com erro e o total de bits transmitidos.  
🔍 Indicador importante para avaliar a qualidade de um link de comunicação, especialmente em redes sem fio ou via satélite.

---

### RTT - Round-Trip Time

**Significado:** Tempo de Ida e Volta  
📌 Tempo que um pacote leva para ir até o destino e voltar com uma resposta.  
🔍 Métrica importante em testes de conectividade e desempenho, como no comando `ping`.

## 🔐 Segurança Digital

### CIA - Confidencialidade, Integridade e Disponibilidade

**Significado:** Confidencialidade, Integridade e Disponibilidade  
📌 Modelo fundamental da segurança da informação.  
- **Confidencialidade**: proteger dados contra acesso não autorizado.  
- **Integridade**: garantir que os dados não sejam alterados indevidamente.  
- **Disponibilidade**: assegurar que os dados estejam acessíveis quando necessários.  
🔍 Utilizado como base para políticas de segurança em empresas e organizações.

---

### SSL - Secure Sockets Layer

**Significado:** Camada de Soquetes Segura  
📌 Protocolo antigo para proteger conexões via criptografia entre cliente e servidor.  
🔍 Hoje é considerado obsoleto, substituído pelo **TLS**, mas o termo "SSL" ainda é amplamente usado para se referir a certificados digitais.

---

### TLS - Transport Layer Security

**Significado:** Segurança da Camada de Transporte  
📌 Protocolo atual e seguro usado para criptografar conexões na web, garantindo integridade e sigilo das comunicações.  
🔍 Utilizado em conexões HTTPS, e-mails, VPNs e outros serviços que exigem segurança de dados.

---

### HTTPS - HyperText Transfer Protocol Secure

**Significado:** Protocolo de Transferência de Hipertexto Seguro  
📌 Versão segura do HTTP, que utiliza o TLS para criptografar a comunicação entre navegador e servidor.  
🔍 Sites com HTTPS protegem seus usuários contra espionagem e ataques como o "man-in-the-middle".

---

### VPN - Virtual Private Network

**Significado:** Rede Privada Virtual  
📌 Cria um túnel criptografado entre o dispositivo do usuário e outro ponto da internet, protegendo a privacidade e permitindo acesso remoto seguro.  
🔍 Usada para acessar redes corporativas ou ocultar a localização em redes públicas.

---

### IDS - Intrusion Detection System

**Significado:** Sistema de Detecção de Intrusão  
📌 Sistema que monitora o tráfego de rede ou atividades do sistema em busca de comportamentos suspeitos.  
🔍 Pode gerar alertas em caso de possíveis ataques ou acessos indevidos.

---

### IPS - Intrusion Prevention System

**Significado:** Sistema de Prevenção de Intrusão  
📌 Semelhante ao IDS, mas com a capacidade de **bloquear** automaticamente atividades maliciosas.  
🔍 Frequentemente usado junto a firewalls para proteção ativa contra ameaças.

---

### MFA - Multi-Factor Authentication

**Significado:** Autenticação Multifator  
📌 Mecanismo de segurança que exige dois ou mais métodos de verificação para conceder acesso a um sistema.  
🔍 Combina algo que o usuário **sabe** (senha), **tem** (celular/token) e **é** (biometria), aumentando a proteção contra acesso indevido.

---

### 2FA - Two-Factor Authentication

**Significado:** Autenticação de Dois Fatores  
📌 Tipo de MFA que utiliza exatamente dois fatores distintos para autenticação.  
🔍 Muito usado em bancos e redes sociais como medida de segurança adicional.

---

### PKI - Public Key Infrastructure

**Significado:** Infraestrutura de Chave Pública  
📌 Sistema que gerencia chaves criptográficas e certificados digitais para comunicação segura.  
🔍 Essencial em sistemas que utilizam criptografia assimétrica, como HTTPS, VPNs e e-mails criptografados.

---

### RSA - Rivest-Shamir-Adleman

**Significado:** Algoritmo de Criptografia RSA  
📌 Algoritmo de criptografia assimétrica muito usado para proteger dados. Usa um par de chaves: pública e privada.  
🔍 Utilizado em protocolos como HTTPS, VPNs, autenticação digital e troca segura de dados.

---

### AES - Advanced Encryption Standard

**Significado:** Padrão Avançado de Criptografia  
📌 Algoritmo de criptografia simétrica muito seguro e rápido, padrão em segurança de dados.  
🔍 Usado em VPNs, criptografia de arquivos, discos rígidos, comunicações seguras, entre outros.

---

### DDoS - Distributed Denial of Service

**Significado:** Negação de Serviço Distribuída  
📌 Ataque em que múltiplos dispositivos comprometidos enviam grandes volumes de tráfego a um sistema-alvo, derrubando-o.  
🔍 Utilizado para tornar sites, servidores ou serviços indisponíveis. Exige mitigação rápida.

---

### MITM - Man In The Middle

**Significado:** Homem no Meio  
📌 Ataque onde o invasor intercepta e possivelmente altera a comunicação entre duas partes sem que elas saibam.  
🔍 Pode ocorrer em conexões sem criptografia (HTTP) ou redes públicas mal protegidas.

---

### CVE - Common Vulnerabilities and Exposures

**Significado:** Vulnerabilidades e Exposições Comuns  
📌 Sistema de catalogação de vulnerabilidades de segurança conhecidas.  
🔍 Cada CVE tem um número único, como CVE-2023-1234, ajudando pesquisadores e empresas a identificarem e corrigirem falhas.

---

### SOC - Security Operations Center

**Significado:** Centro de Operações de Segurança  
📌 Equipe ou local responsável por monitorar e responder a incidentes de segurança em tempo real.  
🔍 Essencial em ambientes corporativos com alto volume de dados e riscos.

---

### SIEM - Security Information and Event Management

**Significado:** Gerenciamento de Informações e Eventos de Segurança  
📌 Sistema que coleta, analisa e correlaciona dados de segurança de diferentes fontes para detectar ameaças.  
🔍 Ajuda analistas de SOC a identificar padrões anômalos e agir rapidamente.

---

### CAPTCHA - Completely Automated Public Turing test to tell Computers and Humans Apart

**Significado:** Teste de Turing Público Automatizado para Diferenciar Computadores e Humanos  
📌 Mecanismo de segurança que exige que o usuário prove que é humano (ex: identificar imagens, digitar letras embaralhadas).  
🔍 Usado para evitar que bots abusem de formulários, cadastros, sistemas de login etc.

