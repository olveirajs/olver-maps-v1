# olver-maps

Two SA-MP maps released for free to the community.  
Dois mapas para SA-MP liberados de graça para a comunidade.

---

## Maps / Mapas

### Prefeitura Municipal
City hall with detailed exterior and interior.  
Prefeitura com exterior e interior detalhados.

- **638 objects / objetos**
- Location / Localização: San Fierro — `X: -2873.13  Y: 422.74  Z: 4.14`
- File / Arquivo: [`prefeitura/prefeitura.pwn`](prefeitura/prefeitura.pwn)

### Concessionária de Veículos
Car dealership with showroom and parking.  
Concessionária com showroom e estacionamento.

- **353 objects / objetos**
- Location / Localização: Las Venturas — `X: -2383.75  Y: -47.53  Z: 36.90`
- File / Arquivo: [`concessionaria/concessionaria.pwn`](concessionaria/concessionaria.pwn)

---

## Requirements / Requisitos

- SA-MP 0.3.7+
- [Streamer Plugin](https://github.com/samp-incognito/samp-streamer-plugin)

---

## Installation / Instalação

**1.** Install the Streamer plugin if you haven't already.  
**1.** Instale o plugin Streamer caso ainda não tenha.

**2.** Add at the top of your gamemode / Adicione no topo do seu gamemode:

```pawn
#include <streamer>
```

**3.** Copy the `.pwn` file content into your gamemode and call the function inside `OnGameModeInit`.  
**3.** Copie o conteúdo do arquivo `.pwn` para o seu gamemode e chame a função dentro do `OnGameModeInit`:

```pawn
public OnGameModeInit()
{
    Map_Prefeitura();
    Map_Concessionaria();
    return 1;
}
```

**4.** Prefeitura only — add inside `OnPlayerConnect` / Apenas para a Prefeitura — adicione dentro do `OnPlayerConnect`:

```pawn
public OnPlayerConnect(playerid)
{
    RemoveBuildingForPlayer(playerid, 1308, -2381.790, -40.414, 34.625, 0.250);
    return 1;
}
```

> This removes a native GTA:SA building that overlaps the map.  
> Isso remove uma construção nativa do GTA SA que sobrepõe o mapa.

---

## Editable / Editável

Both maps are fully editable. You can move, remove or add objects freely to adapt them to your server.  
Os dois mapas são totalmente editáveis. Você pode mover, remover ou adicionar objetos livremente para adaptar ao seu servidor.

---

## Screenshots

### Concessionária de Veículos

| | |
|---|---|
| ![Frente](https://media.discordapp.net/attachments/1500504969458225405/1501077271556132995/sa-mp-001.png?ex=69fac2a6&is=69f97126&hm=66b81439acc6b1961db1cf691181b33ffba4e1841968706b59eaf38a7bf4324c&=&format=webp&quality=lossless&width=1252&height=704) | ![Interior](https://media.discordapp.net/attachments/1500504969458225405/1501077287444152440/sa-mp-002.png?ex=69fac2a9&is=69f97129&hm=8c98937fb3a83ed188aff854a0cffd1f2b06cf3ad69ab663d1b422239cd5c565&=&format=webp&quality=lossless&width=1252&height=704) |
| ![Interior v2](https://media.discordapp.net/attachments/1500504969458225405/1501077305290658002/sa-mp-003.png?ex=69fac2ae&is=69f9712e&hm=b7a6c5dca04a8f1400bb80e993728188d0207d1b64c66178f92318d2d66b8278&=&format=webp&quality=lossless&width=1252&height=704) | |

### Prefeitura Municipal

| | |
|---|---|
| ![Frente](https://media.discordapp.net/attachments/1500504969458225405/1501077322546286602/sa-mp-004.png?ex=69fac2b2&is=69f97132&hm=abb03a624a8d8bdab675a7da46f72cb0689b5a4570d6a713ff58ffb0792af169&=&format=webp&quality=lossless&width=1252&height=704) | ![Próximo](https://media.discordapp.net/attachments/1500504969458225405/1501077338039783494/sa-mp-005.png?ex=69fac2b6&is=69f97136&hm=b2dbbfcc6092363476d1494304ebdcf2e88935e0c3640cf7ec03619e6b66a3c1&=&format=webp&quality=lossless&width=1252&height=704) |
| ![Interior](https://media.discordapp.net/attachments/1500504969458225405/1501077359875588216/sa-mp-006.png?ex=69fac2bb&is=69f9713b&hm=47c7dd7d5c060e0dfcc6b0cce877cbb8cc3cea496824a8dcc7d2eb5cabb437d5&=&format=webp&quality=lossless&width=1252&height=704) | ![Interior v2](https://media.discordapp.net/attachments/1500504969458225405/1501077377256783872/sa-mp-007.png?ex=69fac2bf&is=69f9713f&hm=5e6cfb269807b96ecaa260ce27152c8476e41baf1b672fb9e1156ecb317d12e1&=&format=webp&quality=lossless&width=1252&height=704) |

---

## Credits / Créditos

Maps purchased from / Mapas adquiridos na [loja](https://discord.gg/gz2wWPftK7), released to the community by / liberados para a comunidade por [olveirajs](https://github.com/olveirajs).

---

## License / Licença

MIT — free to use in any server, public or private.  
MIT — livre para usar em qualquer servidor, público ou privado.
