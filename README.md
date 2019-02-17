Usaremos un IDE compatible con Solidity y una testnet local para el despliegue de nuestros contratos.

**NodeJS** en la versión 8 o superior:
Lo utilizaremos tanto para trabajar con Solidity como para montar el API básica para atacar el Smart Contract.

Recomiendo usar NVM para gestión de NodeJS y sus versiones.

----
wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.34.0/install.sh | bash

----

Y a continuación hacemos un export:

----
export NVM_DIR="${XDG_CONFIG_HOME/:-$HOME/.}nvm"

[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
----


----
nvm install node
----




_Si dispara un error en el certificado debemos registrar npm:
_
----
npm config set registry http://registry.npmjs.org/
----

Ganache (de Truffle): No es estrictamente necesario tener la testnet de Ganache, pero nos va a permitir gráficamente ver qué está pasando dentro de la blockchain.

----
npm install ganache-cli
----


También lo tienes disponible para compilarlo desde la versión de Github en https://github.com/trufflesuite/ganache