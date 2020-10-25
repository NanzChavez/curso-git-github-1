
# Conexión a repositorios remotos

Veremos una conexión a un repositorio remoto de diferentes formas, la primera y la más simple, haciendo un clon del repositorio con la instrucción `git clone` y la segunda y un poco más interesante, con la instrucción `git remote`. 

### Hacer un clon del repositorio remoto

Se descarga el repositorio `curso-git-github` .
```bash
git clone https://github.com/jersonmartinez/curso-git-github.git
```
---

### Realizar una conexión de un repositorio local a uno remoto

Se crea un directorio donde se desea conectar el repositorio de git local con el remoto. También se podría crear el directorio con el mismo nombre del repositorio remoto. 

Se inicializa un repositorio: 
```bash
git init
```

Se agrega la ruta de un repositorio y se crea una conexión: 
```bash
git remote add curso-git https://github.com/jersonmartinez/curso-git-github.git
```

Comprobar la conexión de la siguiente manera: 
```bash
git remote
git remote show
git remote -v
git remote --verbose
```

Descargar objetos y referencias del repositorio remoto: 
```bash
git fetch curso-git
```

Se procede a hacer un `pullmerge` ,  o bien, una adaptación de los datos a tu repositorio local: 
```bash
git pull curso-git main
```

Otra forma elegante de hacer lo anterior, es haciendo un `` para combinar los datos de la rama por omisión del repositorio remoto con la rama del repositorio local.
```bash
git merge curso-git/master
```

Para publicar cambios, se tendrá que realizar de la siguiente manera: 
```bash
git push --set-upstream curso-git master
```
---

`Buen café, buen código`

**SOBRE EL AUTOR**

✔ Ing. Jerson Martínez ( 💌 jersonmartinezsm@gmail.com )

<a href="https://www.fulldevops.es/?suscribirse" target="_blank"><img alt="FullDevOps" src="https://img.shields.io/twitter/url?color=9cf&label=%40FullDevOps&logo=FullDevOps&logoColor=informational&style=for-the-badge&url=https%3A%2F%2Ftwitter.com%2Fantoniomorenosm"></a>
<a href="https://www.youtube.com/user/gvideosmtutorialesgm/videos" target="_blank"><img alt="YouTube Channel - Core Stack" src="https://img.shields.io/twitter/url?color=red&label=%40Core%20Stack&logo=Side%20Master&logoColor=yellow&style=for-the-badge&url=https%3A%2F%2Ftwitter.com%2Fantoniomorenosm"></a>
<a href="https://www.youtube.com/user/sidemastersupremo/videos" target="_blank"><img alt="YouTube Channel - Side Master" src="https://img.shields.io/twitter/url?color=red&label=%40Side%20Master&logo=Side%20Master&logoColor=yellow&style=for-the-badge&url=https%3A%2F%2Ftwitter.com%2Fantoniomorenosm"></a>

<a href="https://www.linkedin.com/in/jersonmartinezsm/" target="_blank"><img alt="LinkedIn URL" src="https://img.shields.io/twitter/url?label=Ing.%20Jerson%20Mart%C3%ADnez&logo=linkedin&style=social&url=https%3A%2F%2Fwww.linkedin.com%2Fin%2Fjersonmartinezsm%2F"></a>
<a href="https://twitter.com/antoniomorenosm" target="_blank"><img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/antoniomorenosm?label=S%C3%ADgueme%20en%20%40antoniomorenosm&style=social"></a>

