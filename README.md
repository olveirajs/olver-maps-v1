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
| ![](https://raw.githubusercontent.com/olveirajs/olver-maps-v1/main/screenshots/sa-mp-001.png) | ![](https://raw.githubusercontent.com/olveirajs/olver-maps-v1/main/screenshots/sa-mp-002.png) |
| ![](https://raw.githubusercontent.com/olveirajs/olver-maps-v1/main/screenshots/sa-mp-003.png) | ![](https://raw.githubusercontent.com/olveirajs/olver-maps-v1/main/screenshots/sa-mp-008.png) |

### Prefeitura Municipal

| | |
|---|---|
| ![](https://raw.githubusercontent.com/olveirajs/olver-maps-v1/main/screenshots/sa-mp-004.png) | ![](https://raw.githubusercontent.com/olveirajs/olver-maps-v1/main/screenshots/sa-mp-005.png) |
| ![](https://raw.githubusercontent.com/olveirajs/olver-maps-v1/main/screenshots/sa-mp-006.png) | ![](https://raw.githubusercontent.com/olveirajs/olver-maps-v1/main/screenshots/sa-mp-007.png) |

---

## Credits / Créditos

Maps purchased from / Mapas adquiridos na [loja](https://discord.gg/gz2wWPftK7), released to the community by / liberados para a comunidade por [olveirajs](https://github.com/olveirajs).

---

## License / Licença

MIT — free to use in any server, public or private.  
MIT — livre para usar em qualquer servidor, público ou privado.
