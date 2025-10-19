# Contrato erc-20
Lo primero es entrar al asistente de OpenZeppelin la cual nos ayudara a generar el contrato inteligente:
https://wizard.openzeppelin.com/#erc721 .

A continuación nos saldra la siguiente pagina en la cual podremos activar extensiones opcionales


|Opción	|Descripción|
| ------------- |:-------------:|
|Mintable|Permite crear más tokens después del despliegue |
|Burnable|Permite destruir (quemar) tokens.|
|Pausable|Permite pausar todas las transferencias .|
|Permit |Permite aprobar transferencias sin gastar gas (firma fuera de la cadena).|
|Callback|Admite la ejecución de código después de las transferencias y aprobaciones de los contratos de los destinatarios en una sola transacción.|
|Flash Minting|Préstamos flash integrados. Presta tokens sin garantía, siempre que se devuelvan en la misma transacción.|
|Votes	|Convierte el token en uno con funciones de gobernanza (DAO, votaciones, etc.).|
### Access Control
|Opción	|Descripción|
| ------------- |:-------------:|
|Ownable|Mecanismo simple con una única cuenta autorizada para todas las acciones privilegiadas.|
|Roles|Mecanismo flexible con un rol independiente para cada acción privilegiada. Un rol puede tener varias cuentas autorizadas.|
|Managed|Permite que un contrato central defina una política que permita a ciertos llamantes acceder a ciertas funciones.|

## Creación del token
Seleccionaremos las opciones de "mintable" y "ownable", cambiaremos el nombre del Token y su simbolo, ademas tendremos un premint de 1000.

Creamos el archivo "CCDToken.sol" en Remix IDE y copiamos el codigo generado por OpenZeppelin.

Compilamos el contrato inteligente y los deployamos en la testnet de prueba Sepolia.


