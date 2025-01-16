# bgprr
API bgpview.io

### Requisitos:
```apt install python3-requests python3-tabulate wget```

### Instalação Servidor Remontti:
```
wget remontti.com.br/bgprr -O /bin/bgprr
chmod +x /bin/bgprr
```
### Instalação Servidor Github:
```
wget https://raw.githubusercontent.com/remontti/bgprr/refs/heads/main/bgprr -O /bin/bgprr
chmod +x /bin/bgprr
```

### Uso: 
```
bgprr
Insira um ASN (por exemplo, 15169) ou um nome para pesquisar: netflix
Procurando por ASNs correspondentes 'netflix'...

╒═══════╤═════════════╤════════╤═══════╕
│ AS    │ Nome        │ País   │ Rir   │
╞═══════╪═════════════╪════════╪═══════╡
│ 40027 │ NETFLIX-ASN │ US     │ ARIN  │
╘═══════╧═════════════╧════════╧═══════╛
```

```
bgprr 
Insira um ASN (por exemplo, 15169) ou um nome para pesquisar: 53218
╒═════════════════════════════════════╕
│ AS 65530 - BR - Lacnic - 28/10/2010 │
│ PROVEDOR TELECOMUNICACOES LTDA      │
│ Site: https://www.provedor.com.br   │
│ Contatos: noc@provedor.com.br       │
╘═════════════════════════════════════╛
╒═════════════════════╕
│ Prefixos IPv4       │
╞═════════════════════╡
│ ✅ 192.168.100.0/22 │
│ ✅ 192.168.100.0/23 │
│ ✅ 192.168.100.0/23 │
│ ✅ 192.168.100.0/24 │
╘═════════════════════╛
╒═══════════════════════╕
│ Prefixos IPv6         │
╞═══════════════════════╡
│ ✅ 2001:db8::/32      │
│ ✅ 2001:db8::/33      │
│ ✅ 2001:db8:8000::/33 │
╘═══════════════════════╛
RPKI ✅/❌

Upstreams:
╒═══════╤═══════════════╤════════╤════════╤════════╕
│ ASN   │ Nome          │ País   │ IPv4   │ IPv6   │
╞═══════╪═══════════════╪════════╪════════╪════════╡
│ 65531 │ NET TELECOM   │ BR     │ ✅     │ ✅     │
├───────┼───────────────┼────────┼────────┼────────┤
│ 6939  │ HURRICANE     │ US     │ ✅     │ ✅     │
╘═══════╧═══════════════╧════════╧════════╧════════╛

Downstreams:
╒════════╤═══════════════════════════════════════╤════════╤════════╤════════╕
│ ASN    │ Nome                                  │ País   │ IPv4   │ IPv6   │
╞════════╪═══════════════════════════════════════╪════════╪════════╪════════╡
│ 65532  │ Net Provedor de Internet Ltda         │ BR     │ ✅     │ ❌     │
╘════════╧═══════════════════════════════════════╧════════╧════════╧════════╛

IXs:
╒═════════════════════════════╤════════╤═════════════════╤═════════════════╤═══════════════════════╤══════════════╕
│ Nome                        │ País   │ Cidade          │ IPv4            │ IPv6                  │ Velocidade   │
╞═════════════════════════════╪════════╪═════════════════╪═════════════════╪═══════════════════════╪══════════════╡
│ IX.br (PTT.br) São Paulo    │ BR     │ São Paulo/SP    │ 187.16.216.x    │ 2001:12f8::x          │ 10.00 Gbps   │
├─────────────────────────────┼────────┼─────────────────┼─────────────────┼───────────────────────┼──────────────┤
│ IX.br (PTT.br) Curitiba     │ BR     │ Curitiba        │ 200.219.140.x   │ 2001:12f8:0:4::x      │ 10.00 Gbps   │
├─────────────────────────────┼────────┼─────────────────┼─────────────────┼───────────────────────┼──────────────┤
│ IX.br (PTT.br) Porto Alegre │ BR     │ Porto Alegre/RS │ 177.52.38.x     │ 2001:12f8:0:6::5:x    │ 1.00 Gbps    │
╘═════════════════════════════╧════════╧═════════════════╧═════════════════╧═══════════════════════╧══════════════╛
```

Autor: Rudimar Remontti + GPT
