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
- 
