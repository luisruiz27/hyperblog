# hyperblog
Blog para el curso github Platzi

## Create keys Public and Private
###################### GENERACION DE LLAVES SSH  - WINDOWS ###############################
#Generar una nueva llave SSH: (Cualquier sistema operativo)

```bash
  ssh-keygen -t rsa -b 4096 -C "youremail@example.com"
```
#Comprobar proceso y agregarlo (Windows)
```bash
  eval $(ssh-agent -s)
  ssh-add ~/.ssh/id_rsa
```
###################### GENERACION DE LLAVES SSH  - MAC ###############################
##Comprobar proceso y agregarlo (Mac)
```bash
  eval "$(ssh-agent -s)"
```

# macOS Sierra 10.12.2 o superior, Haz lo siguiente:
```bash
  ssh-add -K ~/.ssh/id_rsa
  cd ~/.ssh
```
# Crea un archivo config
```bash
  Con Vim vim config
  Con VSCode code config
```
#Pega la siguiente configuración en el archivo Host *
```bash
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_rsa
```
  #Agrega tu llave
```bash
  ssh-add -K ~/.ssh/id_rsa
```
