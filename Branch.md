
# 📚 Documentación: Uso de Branches en Git y GitHub

## 📌 ¿Qué es una rama (branch)?

Una **rama** en Git es una versión paralela del proyecto. Se utiliza para trabajar en funciones nuevas, corregir errores o probar ideas, sin afectar la rama principal (`main` o `master`).

---

## 🔧 Comandos básicos para trabajar con ramas

### 1. ✅ Crear una nueva rama

```bash
git branch nombre-de-la-rama
```

Ejemplo:

```bash
git branch editarTexto
```

---

### 2. 🚀 Cambiarse a una rama

```bash
git checkout nombre-de-la-rama
```

O crearla y cambiar a ella directamente:

```bash
git checkout -b nombre-de-la-rama
```

---

### 3. 🔍 Ver las ramas existentes

```bash
git branch
```

Esto muestra todas las ramas locales y cuál estás usando (marcada con `*`).

---

### 4. ⬆️ Subir una rama a GitHub

Después de hacer commits:

```bash
git push -u origin nombre-de-la-rama
```

---

### 5. 🔁 Combinar una rama con `main` (merge)

Primero, cámbiate a la rama `main`:

```bash
git checkout main
```

Luego haz el merge:

```bash
git merge nombre-de-la-rama
```

---

### 6. 🧹 Eliminar una rama

* **Localmente**:

```bash
git branch -d nombre-de-la-rama
```

* **En GitHub (remoto)**:

```bash
git push origin --delete nombre-de-la-rama
```

---

## 🌐 Uso de ramas en GitHub (Interfaz Web)

### Crear una rama nueva:

1. Ve al repositorio.
2. Haz clic en el selector de ramas (generalmente dice `main`).
3. Escribe un nuevo nombre y presiona Enter para crearla.

### Cambiar entre ramas:

* Usa el mismo selector de ramas en la interfaz.

### Crear un Pull Request:

1. Ve a la pestaña **"Pull requests"**.
2. Haz clic en **"New pull request"**.
3. Elige la rama base (`main`) y la rama con tus cambios.
4. Escribe una descripción y crea el PR.

---

## ✅ Buenas prácticas con ramas

* Usa nombres descriptivos:

  * `feature/registro-usuario`
  * `bugfix/login-error`
  * `hotfix/seguridad-urgente`

* Trabaja en ramas pequeñas y específicas.

* Haz Pull Requests antes de mezclar (`merge`) con `main`.

* Borra ramas que ya no usas para mantener limpio el repositorio.

