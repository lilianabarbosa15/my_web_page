## Comandos en git

ASOCIACIÓN DE CLAVE CRIPTOGRAFICA SSH:
- ssh-keygen -t rsa -b 4096 -C "lili_mar1503@hotmail.com"
- ssh-add /c/SPB_Data/.ssh/id_rsa_ssh
- exec ssh-agent bash
- ssh-add /c/SPB_Data/.ssh/id_rsa_ssh
- cat ~/.ssh/id_rsa_ssh.pub


CLONACIÓN DEL REPOSITORIO:
- git clone git@github.com:lilianabarbosa15/my_web_page.git
- cd ./my_web_page

SE CREA NUEVA RAMA:
- git checkout -b new_features

PRIMER COMMIT:
- touch aboutme.html
- (se agrega plantilla)
- git add aboutme.html
- git commit -m "Se acaba de crear un archivo HTML con informacion de la plantilla proporcionada por el profesor"

SEGUNDO COMMIT:
- (se crea directorio)
- touch styles/aboutme.css
- git add styles/aboutme.css
- (se agrega plantilla)
- git commit -m "Se acaba de crear un directorio styles y dentro de el un archivo CSS con la plantilla bàsica proporcionada por el profesor"

TERCER COMMIT:
- (modificacion en aboutme.html)
- git add aboutme.html
- git commit -m "Se acaba de modificar aboutme.html con informacion relevante sobre mi"

CUARTO COMMIT:
- touch index.html
- (se agrega plantilla)
- git add index.html
- git commit -m "Se acaba de crear un archivo index.html, donde se construye lo principal de la pagina web (donde se maneja toda la pagina web)"

QUINTO COMMIT:
- (modificacion en aboutme.html)
- git add aboutme.html
- git commit -m "Se acaba de agregar a la estructura del archivo aboutme.html varios hipertextos relacionados a redes sociales y una referencia a aboutme.css para estilizar el nombre de presentacion"

QUITAR COMMIT DEL PUNTO 15:
- git revert HEAD~1

MERGE CON MAIN:
- git checkout main
- git merge new_features

PUSH AL REPOSITORIO GLOBAL:
- git push --set-upstream origin main
  
