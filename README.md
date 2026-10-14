# tecfri-fpga

Tecfri arcade cores for **MiSTer**. · Cores arcade de **Tecfri** para **MiSTer**.

| Game · Juego | Year · Año | Core | Alternatives · Alternativas |
|---|---|---|---|
| Ambush | 1983 | `ffambush` | hack, Japan, Volt Electronics |
| Hole Land | 1984 | `ffholeland` | Spain |
| Crazy Rally | 1985 | `ffcrzrally` | set 2, Gecas license, Recreativos Franco license |
| Speed Ball | 1987 | `ffspeedbal` | set 2, set 3 |
| Music Ball | 1988 | `ffspeedbal` | |
| Tricky Doc | 1987 | `fftrckydoc` | set 2 |
| Sauro | 1987 | `ffsauro` | set 2, set 3, set 4 (easier), Philko license, Recreativos Real S.A. license, Sea Wolf |

## How to install

Copy the contents of [`_Arcade/`](_Arcade/) to the `_Arcade/` folder of your MiSTer SD card: the `.rbf` files go to
`_Arcade/cores/`, the main `.mra` of each game to `_Arcade/`, and the other sets to `_Arcade/_alternatives/_<Game>/`.

**ROMs are not included.** Bring your own MAME 0.288 **merged** romsets as `.zip` into `games/mame/`: `ambush.zip`,
`holeland.zip`, `crzrally.zip`, `speedbal.zip`, `musicbal.zip`, `trckydoc.zip`, `sauro.zip`. Every set of a game
(main and alternatives) loads from its parent's merged zip.

## Cómo instalar

Copia el contenido de [`_Arcade/`](_Arcade/) a la carpeta `_Arcade/` de la SD de tu MiSTer: los `.rbf` van a
`_Arcade/cores/`, el `.mra` principal de cada juego a `_Arcade/` y el resto de sets a `_Arcade/_alternatives/_<Juego>/`.

**Las ROMs no se incluyen.** Pon tus propios romsets **merged** de MAME 0.288 en `.zip` en `games/mame/`: `ambush.zip`,
`holeland.zip`, `crzrally.zip`, `speedbal.zip`, `musicbal.zip`, `trckydoc.zip`, `sauro.zip`. Todos los sets de un juego
(principal y alternativos) cargan del zip merged de su padre.

## Credits · Créditos

Original cores for the MiSTer framework (`sys/`, GPLv2+). Third-party components inside the `.rbf` files:

- **T80** Z80 CPU — Daniel Wallner (Verilog translation `T80s.v` distributed with JTFRAME, Jose Tejada).
- **jt49** AY-3-8910 — Jose Tejada (GPLv3): Ambush, Hole Land, Crazy Rally.
- **jtopl** YM3812 — Jose Tejada (GPLv3): Speed Ball, Music Ball, Tricky Doc, Sauro.

The SP0256 speech chip (Hole Land, Sauro) is an implementation of its own. License: GPLv3 ([`LICENSE`](LICENSE)).

Cores originales para el framework de MiSTer (`sys/`, GPLv2+). Componentes de terceros dentro de los `.rbf`: los de la
lista anterior. El chip de voz SP0256 (Hole Land, Sauro) es una implementación propia. Licencia: GPLv3 ([`LICENSE`](LICENSE)).
