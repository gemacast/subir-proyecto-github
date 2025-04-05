# subir-proyecto-github
Guía paso a paso para subir cualquier proyecto a GitHub desde Visual Studio Code
# Guía paso a paso: Cómo subir un proyecto a GitHub desde Visual Studio Code

Guía personal para subir un nuevo proyecto a GitHub.

---

## Paso 1: Abrir la terminal en la carpeta del proyecto

Abrir Visual Studio Code, ir a la carpeta donde está mi proyecto y abrir la terminal (`Ver > Terminal` o `Ctrl + ñ`).

Si la carpeta tiene espacios, uso comillas:

```bash
cd "C:\xampp\htdocs\Html a Wordpress\Creacion de plantilla Html\TemaGemma-1"
```

---

## Paso 2: Iniciar Git y hacer el primer commit

Esto convierte mi carpeta en un repositorio Git y guarda la primera versión:

```bash
git init
git add .
git commit -m "Primer commit - estructura base del proyecto"
```

---

##  Paso 3: Crear el repositorio en GitHub

1. Ir a github
2. Hacer clic en  **"New"**
3. Elegir el nombre del repositorio (por ejemplo: `practica3Daw`)
4. **No marcar** la opción *"Add a README"* (porque ya tengo uno local)
5. Clic en **"Create repository"**

---

##  Paso 4: Conectar mi carpeta local con el repositorio de GitHub

Copiar la URL del repositorio (ejemplo):

```
https://github.com/gemacast/practica3Daw.git
```

Pegarla en la terminal así:

```bash
git remote add origin https://github.com/gemacast/practica3Daw.git
git branch -M main
git push -u origin main
```

⚠️ Si ya había un `origin` creado y quiero cambiarlo, primero lo borro:

```bash
git remote remove origin
```

Y luego lo añado de nuevo correctamente.

---

##  Paso 5: Subir cambios nuevos más adelante

Cada vez que modifique archivos y quiera subir los cambios, hago esto:

```bash
git add .
git commit -m "Descripción clara de los cambios realizados"
git push
```

Ejemplo:

```bash
git commit -m "Añadida plantilla front-page.php para la home"
```

---

##  Paso 6: ¿Me pide login?

- Usuario: `mi usuario github`
- Contraseña: si tengo verificación en dos pasos activada, tengo que usar un **Token de Acceso Personal (PAT)** en lugar de la contraseña.

 Si no tengo el token todavía, puedo crearlo aquí:  
[https://github.com/settings/tokens](https://github.com/settings/tokens)

---

## ¡Listo!

Chuleta para consultar  
