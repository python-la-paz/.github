# 🤝 Guía de contribución

¡Gracias por querer contribuir a **Python La Paz**!  
Esta guía explica cómo participar de forma ordenada en cualquiera de nuestros proyectos. Te tomará solo unos minutos leerla y te ayudará a entender cómo funciona nuestro proceso antes de abrir un Issue o enviar un Pull Request.

---

## Índice

- [🤝 Guía de contribución](#-guía-de-contribución)
  - [Índice](#índice)
  - [📜 Código de conducta](#-código-de-conducta)
  - [🚀 ¿Cómo puedo contribuir?](#-cómo-puedo-contribuir)
    - [🤓 Antes de empezar](#-antes-de-empezar)
    - [🐞 Reportar un bug](#-reportar-un-bug)
    - [✨ Sugerir una mejora o nueva funcionalidad](#-sugerir-una-mejora-o-nueva-funcionalidad)
    - [🌱 Tu primera contribución](#-tu-primera-contribución)
    - [📝 Mejorar la documentación](#-mejorar-la-documentación)
  - [🔧 Flujo de trabajo con Git](#-flujo-de-trabajo-con-git)
    - [🔁 Paso a paso para subir tus cambios](#-paso-a-paso-para-subir-tus-cambios)
    - [🌿 Nomenclatura de branches](#-nomenclatura-de-branches)
  - [💻 Estándares de código](#-estándares-de-código)
    - [🐍 Python](#-python)
    - [JavaScript / otros](#javascript--otros)
  - [📝 Mensajes de commit](#-mensajes-de-commit)
    - [Tipos permitidos](#tipos-permitidos)
    - [Ejemplos de mensajes de commit](#ejemplos-de-mensajes-de-commit)
  - [🔍 Proceso de revisión](#-proceso-de-revisión)
    - [✔️ ¿Qué revisamos?](#️-qué-revisamos)
  - [❓ ¿Tienes preguntas?](#-tienes-preguntas)

---

## 📜 Código de conducta

Este proyecto, así como todos los espacios de la comunidad Python La Paz, se rigen por nuestro [Código de Conducta](CODE_OF_CONDUCT.md).

Al participar en cualquiera de nuestros repositorios, actividades o espacios de la comunidad aceptas cumplir con este código. Si observas comportamientos inapropiados o que no respeten estas normas, puedes reportarlos escribiendo a **hello@pylapaz.org**.

---

## 🚀 ¿Cómo puedo contribuir?

### 🤓 Antes de empezar

Antes de comenzar a trabajar en un cambio o proponer una mejora, es importante seguir estos pasos:

1. Verifica si ya existe un Issue relacionado.
2. Si vas a trabajar en un Issue existente, comenta que lo tomarás.
3. Espera confirmación de un **maintainer** si el cambio es grande.

### 🐞 Reportar un bug

Si encontraste un error o comportamiento inesperado en alguno de nuestros proyectos:

1. Ve a la pestaña **Issues** del repositorio correspondiente.
2. Haz clic en **New Issue** y selecciona la plantilla **Bug report**.
3. Completa la información solicitada. Incluye pasos para reproducir el problema, comportamiento esperado, comportamiento actual, versión de Python y sistema operativo.

Mientras más información proporciones, más fácil será reproducir y solucionar el problema.

---

### ✨ Sugerir una mejora o nueva funcionalidad

Si tienes una idea para mejorar el proyecto o agregar una nueva funcionalidad:

1. Ve a la pestaña **Issues** del repositorio correspondiente.
2. Haz clic en **Issue** y selecciona la plantilla **Feature request**.
3. Describe el problema que buscas resolver y la solución que propones.
4. Espera la retroalimentación del equipo antes de comenzar a programar. Esto nos ayuda a evitar trabajo duplicado y a alinear las propuestas con los objetivos del proyecto.

---

### 🌱 Tu primera contribución

Si es tu primera vez contribuyendo a un proyecto open source, puedes comenzar con los issues etiquetados como  
[`good first issue`](https://github.com/search?q=org%3Apython-la-paz+label%3A%22good+first+issue%22+is%3Aopen&type=Issues).

Estas tareas suelen estar bien documentadas y tienen un alcance acotado, por lo que son ideales para familiarizarse con el flujo de trabajo del proyecto.

---

### 📝 Mejorar la documentación

La documentación es tan importante como el código.

Si encuentras algo confuso, incompleto o desactualizado, puedes abrir un Pull Request con la mejora. Las contribuciones a la documentación siempre son bienvenidas.

---

## 🔧 Flujo de trabajo con Git

En nuestros proyectos seguimos el modelo **Fork + Pull Request**.  
Ningún cambio se realiza directamente sobre la rama `main`.

### 🔁 Paso a paso para subir tus cambios

1️⃣ Haz fork del repositorio desde GitHub

2️⃣ Clona tu fork en tu máquina

```bash
git clone https://github.com/TU_USUARIO/NOMBRE_DEL_REPO.git
cd NOMBRE_DEL_REPO
```

3️⃣ Agrega el repositorio original como upstream

```bash
git remote add upstream https://github.com/python-la-paz/NOMBRE_DEL_REPO.git
```

4️⃣ Crea una nueva rama desde `main`

```bash
git checkout -b feat/nombre-de-tu-feature
```

5️⃣ Realiza tus cambios y crea un commit

```bash
git add .
git commit -m "feat: agregar endpoint de autenticación"
```

6️⃣ Actualiza tu rama con los cambios de upstream

```bash
git fetch upstream
git rebase upstream/main
```

7️⃣ Sube tu rama a tu fork

```bash
git push origin feat/nombre-de-tu-feature
```

8️⃣ Ve al repositorio original en GitHub y abre un Pull Request desde tu rama hacia `main` utilizando la **plantilla de Pull Request**.

9️⃣ Completa la información solicitada en la plantilla y envía tu PR para revisión.



### 🌿 Nomenclatura de branches

Esta nomenclatura nos ayuda a identificar rápidamente el propósito de cada rama y a mantener un historial organizado.

| Tipo | Formato | Ejemplo |
|------|---------|---------|
| Nueva funcionalidad | `feat/descripcion` | `feat/login-con-google` |
| Corrección de bug | `fix/descripcion` | `fix/error-al-guardar-evento` |
| Documentación | `docs/descripcion` | `docs/mejorar-readme` |
| Refactoring | `refactor/descripcion` | `refactor/modelo-de-usuario` |
| Tests | `test/descripcion` | `test/cobertura-api-eventos` |

> La descripción de las branches puede estar en español o en inglés, dependiendo del proyecto. Revisa el README.md del repositorio específico para confirmar el idioma preferido.
---

## 💻 Estándares de código

### 🐍 Python

- Seguimos [PEP 8](https://peps.python.org/pep-0008/).
- Los nombres de variables, funciones y clases van **en inglés**; los comentarios y docstrings pueden ir en español.

### JavaScript / otros

Cada repositorio puede tener su propia configuración. Revisa el `README.md` del proyecto específico.

---

## 📝 Mensajes de commit

Usamos [Conventional Commits](https://www.conventionalcommits.org/es/). El formato es:

```text
<tipo>[ámbito opcional]: <descripción>

[cuerpo opcional]

[pie(s) de página opcional(es)]
```

### Tipos permitidos

| Tipo | Cuándo usarlo |
|------|--------------|
| `feat` | Nueva funcionalidad |
| `fix` | Corrección de bug |
| `docs` | Cambios en documentación |
| `style` | Formato, punto y coma, etc. (sin cambios de lógica) |
| `refactor` | Refactoring sin nueva funcionalidad ni bug fix |
| `test` | Agregar o corregir tests |
| `chore` | Tareas de mantenimiento (deps, config, CI/CD) |

### Ejemplos de mensajes de commit

1. **Agregar una nueva funcionalidad:** Imagina que estás trabajando en un proyecto y creas un módulo para login con Google.

    Tu commit se vería así:

    ```bash
    git commit -m "feat(auth): agregar login con Google"
    ```

    👉 Aquí usamos `feat` porque añadimos una nueva funcionalidad.

    👉 El alcance `(auth)` indica que el cambio está en el sistema de autenticación.

    👉 La descripción `agregar login con Google` explica claramente qué se hizo.
2. **Corregir un error:** Descubriste que hay un error al cambiar la fecha de un evento. Después de corregirlo, tu commit podría ser:

    ```bash
    git commit -m "fix(eventos): corregir error al editar fecha de evento"
    ```

    👉 Usamos `fix` porque estamos corrigiendo un bug.

    👉 El alcance `(eventos)` indica que el cambio afecta el módulo de eventos.

    👉 La descripción `corregir error al editar fecha de evento` explica claramente qué se corrigió.

3. **Actualizar la documentación:** Si actualizaste el README para mejorar las instrucciones de instalación, tu commit podría ser:

   ```bash
   git commit -m "docs: actualizar instrucciones de instalación en README"
   ```

    👉 Usamos `docs` porque el cambio es en la documentación.

    👉 La descripción `actualizar instrucciones de instalación en README` explica claramente qué se actualizó.

4. **Refactorizar código:** Reorganizaste funciones sin cambiar la lógica ni añadir nuevas features.

   ```bash
   git commit -m "refactor(utils): simplificar funciones de formato"
    ```

     👉 Usamos `refactor` porque estamos mejorando la estructura del código sin agregar funcionalidades ni corregir bugs.
     
     👉 El alcance `(utils)` indica que el cambio afecta el módulo de utilidades.
     
     👉 La descripción `simplificar funciones de formato` explica claramente qué se refactorizó.

5. **Actualizar dependencias:** Si actualizaste las dependencias a versiones estables, tu commit podría ser:

    ``` bash
    git commit -m "chore(deps): actualizar dependencias a la última versión"
    ```

    👉 Usamos `chore` porque es una tarea de mantenimiento.
    
    👉 El alcance `(deps)` indica que el cambio afecta las dependencias del proyecto.
    
    👉 La descripción `actualizar dependencias a la última versión` explica claramente qué se hizo.

---

## 🔍 Proceso de revisión

1. Cuando abres un PR, al menos **un miembro del equipo de maintainers** revisará los cambios antes de aprobar el merge.
2. Es posible que recibas comentarios o sugerencias de mejora. Esto forma parte normal del proceso de revisión.
3. Una vez aprobado, un **maintainer** hará el merge.
4. Los PRs se mergean usando **Squash and Merge** para mantener el historial limpio.

### ✔️ ¿Qué revisamos?

- ✅ El código cumple con los estándares del proyecto
- ✅ Existen tests cuando el cambio lo requiere
- ✅ La documentación está actualizada
- ✅ El PR tiene una descripción clara de qué hace y por qué
- ✅ El PR está vinculado al issue correspondiente (`Closes #N`)

---

## ❓ ¿Tienes preguntas?

- 💬 Únete a la comunidad de [WhatsApp](https://chat.whatsapp.com/JNcZ1qy3lDZL61sAlJia0j) y [Discord](https://discord.com/invite/TV5tHvdUKt) 
- 📧 Escríbenos: hello@pylapaz.org
- 🌐 Visita: [pylapaz.org](https://pylapaz.org)

---

*Hecho con 🐍❤️ desde La Paz, Bolivia*