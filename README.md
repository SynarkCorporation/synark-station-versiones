# Synark Station · versiones

Aquí se publican los instaladores de **Synark Station**, el programa de Windows de la caja SYNARK.
Las apps instaladas miran este repositorio para actualizarse solas.

- **Descargar:** la última versión está en [Releases](https://github.com/SynarkCorporation/synark-station-versiones/releases/latest). Se baja `Synark-Station-<versión>-setup.exe` y se instala.
- **Actualizaciones:** la app busca una versión nueva al arrancar y cada 4 horas, la descarga sola y la instala al cerrarla.

## Licencia: `licencia.json`

Es el interruptor de la licencia para **todas** las apps instaladas. Se edita aquí mismo (lápiz → «Commit changes»).

| Campo | Qué es |
|---|---|
| `activa` | `false`: licencia apagada en todas las apps. `true`: se enciende en todas (en menos de 6 horas, o al abrirlas). |
| `precioMes` | Precio de una licencia al mes. |
| `moneda` | `EUR`. |
| `movilesPorLicencia` | Móviles que cubre una licencia: una caja SYNARK, 20. |
| `pruebaDias` | Días de prueba gratis desde el día que se enciende. |
| `pruebaMoviles` | Móviles que se pueden usar a la vez en la prueba. |

Ojo: el archivo tiene que seguir siendo JSON válido (comillas dobles, comas entre campos, `true`/`false` sin comillas). Si se rompe, las apps lo ignoran y siguen con lo último que leyeron.
