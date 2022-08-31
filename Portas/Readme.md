# Portas de rede

-------------------

Grupo de portas               | Intervalo de números | Descrição |
:-----------------------------|:--------------------:|-----------|
Portas bem<br>conhecidas      | 0 a 1023             | - Estes números de portas são revervados para serviços comuns ou populares e aplicativos como navegadores da web, clientes de e-mail e acesso remoto clientes.<br> - Portas bem conhecidas definidas para aplicativos comuns de servidor que permitem identificar facilmente o serviço associado necessário.
Portas Registradas            | 1024 a 49151         | - Esses números de portas são atribuídos pela IANA a uma entidade solicitante para usar com processos ou aplicativos específicos.<br> - Esses processos são principalmente aplicativos individuais que um usuário optou por instalar, em vez de aplicativos comuns que recebem números de portas bem conhecidos. 
Particulares e/ou<br>Dinâmicas| 49152 a 65535        | - Essas portas também são conhecidas como portas efêmeras.<br> - O sistema operacional do cliente geralmente atribui números de porta dinamicamente quando uma conexão a um serviço é iniciada.<br> - A porta dinâmica é então usada para identificar o aplicativo cliente durante a comunicação.

-------------------
### Códigos de destino inacessível para ICMPv4:

* 0 - Rede inacessível
* 1 - Host inacessível
* 2 - Protocolo inacessível
* 3 - Porta inacessível

### Códigos de destino inacessível para ICMPv6:

* 0 - Sem rota para o destino
* 1 - Comunicação com o destino é proibida administrativamente (ex: firewall)
* 2 - Além do escopo do endereço de origem
* 3 - Endereço inacessível
* 4 - Porta inacessível

-------------------

#### Camada de aplicação: WWW, HTTP, SMTP, Telnet, FTP, SSH, NNTP, RDP, IRC, SNMP, POP3, IMAP, SIP, DNS, PING
#### Camada de transporte: TCP, UDP, RTP, DCCP, SCTP
#### Camada de ligação física: Ethernet, Modem, PPP, FDDi


Porta | Protocolo | Serviço
:-----|:---------:|:-------:
20/21 |TCP        |FTP
22    |TCP/UDP    |SSH 
23    |TCP/UDP    |TELNET
25    |TCP/UDP    |SMTP
53    |TCP/UDP    |DNS
67/68 |UDP        |DHCP
80    |TCP        |HTTP
110   |TCP        |POP3
123   |UDP        |NTP
135   |TCP        |MSRPC
139   |TCP        |NETBIOS-SSN
143   |TCP        |IMAP4
156   |TCP/UDP    |SQL
161   |TCP/UDP    |SNMP
179   |TCP        |BGP
443   |TCP        |HTTPS
445   |TCP        |MICROSOFT-DS
1723  |TCP/UDP    |TUNEL PPTP
1863  |TCO        |MSN
3128  |TCP        |SQUID
3306  |TCP        |MySQL
3389  |TCP        |TERMINAL SERVER
