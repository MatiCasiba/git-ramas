# Git RAMAS (Bramches)

```sh
git init
```

## Ver el status de los archivos 
```sh
git status
```

## Git Alias
```sh
git config --global alias.st "status --short"
git confg --global alias.a "add"
git confg --global alias.c "commit -m"
git confg --global alias.l "log --oneline"
```

## Ver las diferencias entre el WD(working directory) y LR(local repo)

```sh
git diff
```

# Ver el contenido de cada commit 

```sh
git show <numero-hash>
```

## Crear una rama

```sh
git branch <nombre-rama> #crea una rama y nos deja en la rama actual/original

git branch feature/ramas #ejemplo
git switch -c <nombre-rama> # crea una rama y nos mueve a la rama que se creo
```

## Me mueve entre ramas

```sh
git switch <nombre-rama>
git switch feature/ramas #ejemplo
```

## Comparar entre los ultimos commits de las ramas

```sh
git diff <nombre-rama-que-quiero-comparar> #comparo la rama actual contra la rama que indico
git diff dev # ejemplo. comparo feature/ramas con dev
```

## Ver ramas locales y remotas

```sh
git branch -a # me muestra las ramas locales y remotas
```

## Fucionando ramas
Estoy sobre la rama main y me quiero traer lo que esta en feature ramas
```sh
git merge <rama-que-quiero-fusionar>

git switch main #ejemplo
git merge feature/ramas # Me traigo a main lo que tenia en feature/ramas
```

* Fusión -> Fast-foward -> git hace la fusion automaticamente.


