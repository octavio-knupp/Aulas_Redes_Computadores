# Aulas_Redes_Computadores
# Esboço de aulas de redes ou curiosidades 
- https://www.shorturl.at/tPjoQ.
- Gran Qeustões.com
- https://jodies.de/ipcalc - site para encontrar o ip local
- utilizar a coversão para numero bínario
- coversão de ip sempre será 8 digitos ou byts
- mascara de rede serve: serve para dividir um endereço IP em duas partes: uma parte que identifica a rede e outra que identifica o host (dispositivo) dentro dessa rede. garante segurança
- broadcast é um método de envio de dados onde uma única mensagem é transmitida para todos os dispositivos em uma rede local simultaneamente
- wildcard (ou máscara wildcard) é um padrão de bits usado para indicar quais partes de um endereço IP devem ser correspondidas e quais podem ser ignoradas. É semelhante a uma máscara de sub-rede, mas opera de forma inversa, usando 0s para indicar bits que devem corresponder e 1s para bits que podem ser ignorados.
- tem que aprender a calcular essa merda----->
- Address:   172.27.32.118         10101100.00011011 .00100000.01110110
Netmask:   255.255.0.0 = 16      11111111.11111111 .00000000.00000000
Wildcard:  0.0.255.255           00000000.00000000 .11111111.11111111
=>
Network:   172.27.0.0/16         10101100.00011011 .00000000.00000000 (Class B)
Broadcast: 172.27.255.255        10101100.00011011 .11111111.11111111
HostMin:   172.27.0.1            10101100.00011011 .00000000.00000001
HostMax:   172.27.255.254        10101100.00011011 .11111111.11111110
Hosts/Net: 65534                 (Private Internet)
- https://en.wikipedia.org/wiki/Private_network aprender a tabela desse site
- O DNS (Sistema de Nomes de Domínio) é um sistema que traduz nomes de domínio legíveis por humanos (como www.exemplo.com) em endereços IP numéricos (como 192.0.2.44) que os computadores usam para se comunicarem na internet. É como uma lista telefônica para a internet, onde você procura pelo nome de um site e encontra o endereço IP correspondente.
- TCP/IP (Protocolo de Controle de Transmissão/Protocolo de Internet) é um conjunto de protocolos de comunicação que define como os dados são transmitidos através de redes, incluindo a Internet. Ele funciona dividindo as informações em pacotes e usando o IP para endereçar e direcioná-los aos seus destinos corretos, e o TCP para garantir que todos os pacotes cheguem na ordem correta e sem erros, reestabelecendo a comunicação se necessário.
- HTTP (Hypertext Transfer Protocol)
- HTTPS (Hypertext Transfer Protocol Secure)
- LAN é um acrónimo de Rede de Área Local (Local Area Network), que se refere a uma rede de computadores e outros dispositivos interligados numa área geográfica limitada, como uma casa, escritório ou um único edifício. As LANs permitem o compartilhamento de recursos, como impressoras e ficheiros, e o acesso a uma ligação à internet, usando tecnologias como Ethernet (cabos) ou Wi-Fi (sem fios).
- Uma intranet é uma rede privada usada dentro de uma organização para comunicação interna e compartilhamento seguro de informações. Ela funciona como uma versão privada da Internet, acessível apenas por funcionários autorizados. As intranets são frequentemente usadas para otimizar processos, melhorar a comunicação interna e facilitar o acesso a documentos e ferramentas de trabalho.
- DNS, ou Sistema de Nomes de Domínio (Domain Name System), é um serviço que funciona como a "agenda telefônica" da Internet, traduzindo nomes de domínio legíveis por humanos (como www.google.com) em endereços IP (como 192.0.2.44) que os computadores usam para se comunicar e encontrar sites. Esse processo é fundamental para que os navegadores possam acessar informações na Internet, pois os usuários não precisam memorizar os complexos endereços numéricos dos servidore
- O tráfego SMTP é o tráfego gerado pelo Protocolo Simples de Transferência de Correio (SMTP) para enviar e-mails pela internet, enquanto o DNS (Sistema de Nomes de Domínio) é responsável por traduzir nomes de domínio em endereços IP, um processo essencial para a entrega de e-mails via SMTP, já que o DNS é consultado para encontrar o servidor de e-mail de destino.
- Um firewall é um sistema de segurança (hardware, software ou ambos) que controla o tráfego de rede — decidindo o que entra e o que sai de um computador, servidor ou rede inteira, de acordo com regras pré-definidas.
  Ele funciona como uma barreira entre a rede interna (segura) e a rede externa (não confiável, como a internet)./
-O que é um WAF?
 É uma camada de segurança que fica na frente de uma aplicação web e filtra o tráfego HTTP/HTTPS, identificando e bloqueando ataques típicos de aplicações.


# ARQUITETURAS E ESCALABILIDADE
- 🔌 ARQUITETURA DE REDES

A arquitetura de redes define como os componentes de uma rede de computadores são organizados e como se comunicam. Ela é essencial para garantir eficiência, segurança e desempenho na comunicação entre dispositivos.

1. Componentes Básicos

Dispositivos finais: computadores, smartphones, servidores.

Dispositivos de rede: switches, roteadores, hubs, firewalls.

Meios de transmissão: cabos (fibra, coaxial, par trançado) e sinais sem fio.

2. Tipos de Arquitetura

Cliente-Servidor:

Um servidor central fornece recursos e serviços.

Os clientes solicitam esses serviços.

Exemplo: Web, e-mails, bancos de dados.

Ponto-a-Ponto (P2P):

Todos os dispositivos atuam como cliente e servidor.

Compartilhamento direto de arquivos, por exemplo.

Exemplo: redes Torrent.

Arquitetura em Camadas (Modelo OSI e TCP/IP):

Divide a comunicação em camadas para padronizar funções.

OSI: 7 camadas | TCP/IP: 4 camadas (Aplicação, Transporte, Internet, Acesso à Rede).

📈 ESCALABILIDADE DE REDES

Escalabilidade é a capacidade de uma rede crescer (adicionar mais dispositivos, usuários ou tráfego) sem perda significativa de desempenho.

Tipos de Escalabilidade:
1. Horizontal

Adição de mais dispositivos (ex: mais servidores, switches).

Exemplo: cluster de servidores para balanceamento de carga.

2. Vertical

Potencializa os recursos de um único equipamento (ex: mais memória, processador).

Exemplo: upgrade de um servidor central.

🧩 Boas Práticas para Escalabilidade

Segmentação de redes (VLANs): Reduz o domínio de broadcast.

Balanceamento de carga: Distribui requisições entre servidores.

Redundância e failover: Garante disponibilidade mesmo em falhas.

Uso de protocolos eficientes: Ex: OSPF, BGP para roteamento dinâmico.

Monitoramento constante: Para prever gargalos e agir antes que se tornem problemas.

🌐 Exemplo Prático

Imagine uma empresa crescendo:

Começa com um servidor e 10 computadores (rede simples).

Aumenta para 200 usuários → precisa de VLANs, switches gerenciáveis.

Começa a vender online → adiciona servidores em nuvem e balanceadores de carga.

Expande globalmente → usa CDNs e data centers em outras regiões.

# CAMADAS DE REDES ⚙️
- 1 - Camada Física
 Ver artigo principal: Camada física
A camada física define especificações elétricas e físicas dos dispositivos. Em especial, define a relação entre um dispositivo e um meio de transmissão, tal como um cabo de cobre ou um cabo de fibra óptica. Isso inclui o layout de pinos, tensões, impedância da linha, especificações do cabo, temporização, hubs, repetidores, adaptadores de rede, adaptadores de barramento de host (HBA usado em redes de área de armazenamento) e muito mais. A camada física é responsável por definir se a transmissão pode ser ou não realizada nos dois sentidos simultaneamente. Sendo a camada mais baixa do modelo OSI, diz respeito a transmissão e recepção do fluxo de bits brutos não-estruturados em um meio físico. Ela descreve as interfaces elétricas, ópticas, mecânicas e funcionais para o meio físico e transporta sinais para todas as camadas superiores.

Tem-se que a Camada Física atribui as características mecânicas, elétricas e funcionais, além dos procedimentos para ativar, manter e desativar conexões físicas para a transmissão de bits. Assim, a Camada Física OSI fornece os requisitos para transportar pelo meio físico de rede os bits que formam o quadro da camada de Enlace de Dados, tendo como objetivo, criar o sinal elétrico, óptico ou micro-ondas que representa os bits em cada quadro.

- 2 - Camada de Ligação de Dados ou Enlace de Dados
 Ver artigo principal: Camada de enlace de dados
A camada de ligação de dados também é conhecida como de enlace ou link de dados. Esta camada detecta e, opcionalmente, corrige erros que possam acontecer no nível físico. É responsável por controlar o fluxo (recepção, delimitação e transmissão de quadros) e também estabelece um protocolo de comunicação entre sistemas diretamente conectados.

- 3 - Camada de Rede
 Ver artigo principal: Camada de rede
A camada de rede fornece os meios funcionais e de procedimento de transferência de comprimento variável de dados de sequências de uma fonte de acolhimento de uma rede para um host de destino numa rede diferente (em contraste com a camada de ligação de dados que liga os hosts dentro da mesma rede), enquanto se mantém a qualidade de serviço requerido pela camada de transporte. A camada de rede realiza roteamento de funções, e também pode realizar a fragmentação e remontagem e os erros de entrega de relatório. Roteadores operam nesta camada, enviando dados em toda a rede estendida e tornando a Internet possível. Este é um esquema de endereçamento lógico - os valores são escolhidos pelo engenheiro de rede. O esquema de endereçamento não é hierárquico.

A camada de rede pode ser dividida em três subcamadas:

Sub-rede de acesso - considera protocolos que lidam com a interface para redes, tais como X.25;
Sub-rede dependente de convergência - necessária para elevar o nível de uma rede de trânsito, até ao nível de redes em cada lado;
Sub-rede independente de convergência - lida com a transferência através de múltiplas redes. Controla a operação da sub rede roteamento de pacotes, controle de congestionamento, tarifação e permite que redes heterogêneas sejam interconectadas.
- 4 - Camada de Transporte
 Ver artigo principal: Camada de transporte
A camada de transporte é responsável por receber os dados enviados pela camada de sessão e segmentá-los para que sejam enviados a camada de rede, que por sua vez, transforma esses segmentos em pacotes. No receptor, a camada de Transporte realiza o processo inverso, ou seja, recebe os pacotes da camada de rede e junta os segmentos para enviar à camada de sessão.

Isso inclui controle de fluxo, ordenação dos pacotes e a correção de erros, tipicamente enviando para o transmissor uma informação de recebimento, garantindo que as mensagens sejam entregues sem erros na sequência, sem perdas e duplicações.

A camada de transporte separa as camadas de nível de aplicação (camadas 5 a 7) das camadas de nível físico (camadas de 1 a 3). A camada 4, Transporte, faz a ligação entre esses dois grupos e determina a classe de serviço necessária como orientada à conexão, com controle de erro e serviço de confirmação ou sem conexões e nem confiabilidade.

O objetivo final da camada de transporte é proporcionar serviço eficiente, confiável e de baixo custo. O hardware e/ou software dentro da camada de transporte e que faz o serviço é denominado entidade de transporte.

A entidade de transporte comunica-se com seus usuários através de primitivas de serviço trocadas em um ou mais TSAP (Transport Service Access Point), que são definidas de acordo com o tipo de serviço prestado: orientado ou não à conexão. Estas primitivas são transportadas pelas TPDU (Transport Protocol Data Unit).

Na realidade, uma entidade de transporte poderia estar simultaneamente associada a vários TSA e NSAP (Network Service Access Point). No caso de multiplexação, associada a vários TSAP e a um NSAP e no caso de splitting, associada a um TSAP e a vários NSAP.

A ISO define o protocolo de transporte para operar em dois modos:

Orientado à conexão
Não-Orientado à conexão.
Como exemplo de protocolo orientado à conexão, temos o TCP, e de protocolo não orientado à conexão, temos o UDP. É óbvio que o protocolo de transporte não orientado à conexão é menos confiável. Ele não garante - entre outras coisas - a entrega das TPDU, nem tão pouco a ordenação das mesmas. Entretanto, onde o serviço da camada de rede e das outras camadas inferiores é bastante confiável - como em redes locais - o protocolo de transporte não orientado à conexão pode ser utilizado, sem o overhead inerente a uma operação orientada à conexão.

O serviço de transporte baseado em conexões é semelhante ao serviço de rede baseado em conexões. O endereçamento e controle de fluxo também são semelhantes em ambas as camadas. Para completar, o serviço de transporte sem conexões também é muito semelhante ao serviço de rede sem conexões. Constatado os fatos acima, surge a seguinte questão: "Por que termos duas camadas e não uma apenas?". A resposta é sutil, mas procede: A camada de rede é parte da sub-rede de comunicações e é executada pela concessionária que fornece o serviço (pelo menos para as WAN). Quando a camada de rede não fornece um serviço confiável, a camada de transporte assume as responsabilidades, melhorando em suma importância a qualidade do serviço.

- 5 - Camada de Sessão
 Ver artigo principal: Camada de sessão
Responsável pela troca de dados e a comunicação entre hosts, a camada de Sessão permite que duas aplicações em computadores diferentes estabeleçam uma comunicação, definindo como será feita a transmissão de dados, pondo marcações nos dados que serão transmitidos. Se porventura a rede falhar, os computadores reiniciam a transmissão dos dados a partir da última marcação recebida pelo computador receptor.

- 6 - Camada de Apresentação
 Ver artigo principal: Camada de apresentação
A camada de Apresentação, também chamada camada de Tradução, converte o formato do dado recebido pela camada de Aplicação em um formato comum a ser usado na transmissão desse dado, ou seja, um formato entendido pelo protocolo usado. Um exemplo comum é a conversão do padrão de caracteres (código de página) quando o dispositivo transmissor usa um padrão diferente do ASCII. Pode ter outros usos, como compressão de dados e criptografia.

Os dados recebidos da camada 7 estão descomprimidos, e a camada 6 do dispositivo transmissor fica responsável por comprimir esses dados. A transmissão dos dados torna-se mais rápida, já que haverá menos dados a serem transmitidos: os dados recebidos da camada 4 foram "encolhidos" e enviados à camada 1.

Para aumentar a segurança, pode-se usar algum esquema de criptografia neste nível, sendo que os dados só serão descodificados na camada 6 do dispositivo receptor.

Ela trabalha transformando os dados em um formato no qual a camada de aplicação possa aceitar, minimizando todo tipo de interferência.

- 7 - Camada de Aplicação
 Ver artigo principal: Camada de aplicação
A camada de aplicação corresponde às aplicações (programas) no topo da camada OSI que serão utilizadas para promover uma interação entre a máquina-usuário (máquina destinatária e o usuário da aplicação). Esta camada também disponibiliza os recursos (protocolo) para que tal comunicação aconteça, por exemplo, ao solicitar a recepção de e-mail através do aplicativo de e-mail, este entrará em contato com a camada de Aplicação do protocolo de rede efetuando tal solicitação (POP3 ou IMAP).

Tudo nesta camada é relacionado ao software. Alguns protocolos utilizados nesta camada são: HTTP, SMTP, FTP, Telnet, SIP, RDP, IRC, SNMP, NNTP, POP3, IMAP, BitTorrent, DNS, ICMP.

# HELLO WORD
