# Aulas_Redes_Computadores
# Esboço de aulas de redes ou curiosidades 
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
# ARQUITETURAS E ESCALABILIDADE
- 
