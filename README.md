# PASOS A SEGUIR:

-Primer paso: Modificamos algo en la main y lo añadimos 
como A con los siguientes comandos.

```
git add Main.Java
git commit -m "A"
```
-Segundo paso: Modificamos otra cosa en la main y lo añadimos
como B con los siguientes comandos.
```
git add Main.Java
git commit -m "B"
```

-Tercer paso: Creamos una branch nueva a la que llamaremos exp,
una clase con el mismo nombre, hacemos un checkout a esa rama
y a continuación hacemos una modificacion en 
esa clase que añadimos como C con los siguientes comandos.
```
git branch exp
git checkout exp
git add exp.Java
git commit -m "C"
```

-Cuarto paso: Vamos a la rama master con un checkout, modificamos
algo en la main y lo añadimos como E con los siguientes comandos.

```
git checkout master
git add Main.Java
git commit -m "E"
```
-Quinto paso: Vamos a la rama exp con un checkout, modificamos
algo en la clase exp y lo añadimos como D con los siguientes comandos.
```
git checkout exp
git add exp.Java
git commit -m "D"
```
-Sexto paso: Vamos a la rama master con un checkout, y hacemos un merge
con un comentario que llamamos F con los siguientes comandos.
```
git checkout master
git merge exp -m "F"
```
