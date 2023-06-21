# Activar MFA en tu cuenta AWS

Como medida de seguridad es necesario activar la autenticación multifactor (MFA), en esta pequeña guía veremos los pasos a seguir para su habilitación.

<p align="center">
  <img src="images/1.webp" />
</p>

## Prerequisito:

Tener instalado Google Authenticator(Mobile) o Authy (Mobile o desktop), en esta guía usaremos Authy Desktop

Ingresar a la consola de AWS Services:

<p align="center">
  <img src="images/2.webp" />
</p>

Ingresar la contraseña

<p align="center">
  <img src="images/3.webp" />
</p>

Una vez iniciada la sesión, el campo de búsqueda de servicios escribir IAM

<p align="center">
  <img src="images/4.webp" />
</p>

Hacer click en el primer resultado

Nos muestra una advertencia en la que se nos sugiere activar MFA para el usuario root.

<p align="center">
  <img src="images/5.webp" />
</p>

Hacer click en el botón Add MFA, ingresar un nombre para el dispositivo

<p align="center">
  <img src="images/6.webp" />
</p>

Escoger el tipo de dispositivo, en este caso usaremos Authenticator app, hacer click en Next

<p align="center">
  <img src="images/7.webp" />
</p>

Hacer click en el texto Show secret key, copiarlo

<p align="center">
  <img src="images/8.webp" />
</p>

Abrir Authy Desktop, hacer click en el botón +

<p align="center">
  <img src="images/9.webp" />
</p>

Pegar el código previamente obtenido

<p align="center">
  <img src="images/10.webp" />
</p>

Hacer click en Add Account, ingresar un nombre para la cuenta, escoger un logotipo acorde al servicio, en este caso Amazon Web Services, hacer click en Save

<p align="center">
  <img src="images/11.webp" />
</p>

Copiar el código generado por Authy Desktop y pegarlo en la consola de AWS Services

<p align="center">
  <img src="images/code.webp" />
</p>

Esperar a que genere el segundo código para repetir el anterior paso y hacer click en el botón Add MFA

<p align="center">
  <img src="images/13.webp" />
</p>

¡Excelente!, cada vez que inicies sesión en tu cuenta tendras que ir a Authy para confirmar la doble autenticación.