# Networks

-------------------

### Classes de redes (ipv4):

Classe de endereçamento | intervalo 1º octeto | Máscara de rede|
:----------------------:|:-------------------:|:--------------:|
Classe A                | 1 - 126             | 255.0.0.0      | 
Classe B                | 128 - 191           | 255.255.0.0    |
Classe C                | 192 - 223           | 255.255.255.0  |
Classe D                | 224 - 239           | -              |
Classe E                | 240 - 255           | -              | 

* **Padrao classful**
1. As Classes A, B e C são utilizadas pelos dispositivos

2. Classe D - Utilizada para multicast

3. Classe E  - Utilizada para testes (Hj não é utilizada)

-------------------

### Subredes:

Slash (CIDR) |      Mask     | sub-redes | total de ips | Calculo da mask|
:------------|---------------|:---------:|:------------:|:--------------:|
/25          |255.255.255.128|  2        |  128         | 128            |
/26          |255.255.255.192|  4        |  64          | 128 + 64 = 192 |
/27          |255.255.255.224|  8        |  32          | 192 + 32 = 224 | 
/28          |255.255.255.240|  16       |  16          | 224 + 16 = 240 |
/29          |255.255.255.248|  32       |  8           | 240 + 8 = 248  |
/30          |255.255.255.252|  64       |  4           | 248 + 4 = 252  |

#### Calculando uma subrede (exemplo):

* Ip de exemplo: 198.5.3.0
* Slash: /26
* 64 ips por subnet

| Ordem | Primeiro ip de cada rede | Broadcast |    
:-------|:------------------------:|:---------:|      
Rede 1  | 198.5.3.0                |198.5.3.63 | 
Rede 2  |  ... .3.64               |... .3.127 |
Rede 3  |  ... .3.128              |... .3.191 |
Rede 4  |  ... .3.192              |... .3.255 |

Calcule primeiramente o IP de cada rede, depois utilize o ip das demais redes e subtraia em 1 para encontrar o broadcast

Um endereço sempre será reservado para a rede e um para o broadcast.

Como boa prática, o primeiro IP será o da rede e o último o broadcast.

-------------------


