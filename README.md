# samp-open-maps

Two SA-MP maps released for free to the community.

> Dois mapas para SA-MP liberados de graça para a comunidade.

---

## Maps

### Prefeitura Municipal
City hall with detailed exterior and interior.  
Prefeitura com exterior e interior detalhados.

- **638 objects**
- Location: San Fierro — `X: -2873.13  Y: 422.74  Z: 4.14`
- File: [`prefeitura/prefeitura.pwn`](prefeitura/prefeitura.pwn)

### Concessionária de Veículos
Car dealership with showroom and parking.  
Concessionária com showroom e estacionamento.

- **353 objects**
- Location: Las Venturas — `X: -2383.75  Y: -47.53  Z: 36.90`
- File: [`concessionaria/concessionaria.pwn`](concessionaria/concessionaria.pwn)

---

## Requirements

- SA-MP 0.3.7+
- [Streamer Plugin](https://github.com/samp-incognito/samp-streamer-plugin)

---

## Installation

**1.** Install the Streamer plugin if you haven't already.

**2.** Add at the top of your gamemode:

```pawn
#include <streamer>
```

**3.** Copy the `.pwn` file content into your gamemode and call the function inside `OnGameModeInit`:

```pawn
public OnGameModeInit()
{
    Map_Prefeitura();
    Map_Concessionaria();
    return 1;
}
```

**4.** Prefeitura only — add inside `OnPlayerConnect`:

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

## Credits

Maps purchased from [this store](https://discord.gg/gz2wWPftK7), released to the community by [olveirajs](https://github.com/olveirajs).

---

## License

MIT — free to use in any server, public or private.
