# Prueba de Git desde la terminal

Para clonar tu fork de el repo:
``` {bash}
git clone "tu fork"
```

Ya que hiciste eso, para que puedas actualizar tu version, hay que poner: (solo una vez)
```
git remote add principal https://github.com/Ingenieria-de-Software-ITAM-2020/Softwerinos
```


Para actualizar mi version:
```
git pull principal main
git push origin main
```

Ya que actualizaste, puedes editar todo desde tu compu.
Para abrir vsCode
```
code .
```

Para hacer un commit:
```
git add .
git commit -m "El mensaje que quieras subir"
git push
```
Ya que tenemos el commit, hay que hacer el pull request desde github.com
