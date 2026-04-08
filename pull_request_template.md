---
name: Pull Request
about: Abre un Pull Request para contribuir con código, documentación o pruebas
title: "[PR]"
labels: enhancement
assignees: ""
---
<!-- Gracias por contribuir a Python La Paz 🐍
     Antes de enviar tu PR, asegúrate de haber leído el CONTRIBUTING.md:
     https://github.com/python-la-paz/.github/blob/main/CONTRIBUTING.md -->

## ✨ Descripción

<!-- Explica qué hace este PR y por qué es necesario.
     Una buena descripción responde: ¿qué cambiaste?, ¿por qué?, ¿cómo lo hiciste?
     Ej: "Agrega validación del número de serie en el endpoint POST /billetes 
     para evitar que se procesen entradas vacías, lo que causaba un error 500." -->

## 🔄 Tipo de cambio

<!-- Marca con una X todos los que apliquen -->

- [ ] 🐛 **Bug fix** - corrección de un problema existente
- [ ] 🚀 **Nueva funcionalidad** - agrega algo nuevo sin romper lo existente
- [ ] 💥 **Breaking change** - modifica comportamiento existente
- [ ] 📄 **Documentación** - cambios solo en docs, README o comentarios
- [ ] 🎨 **Estilo / Refactor** - mejoras de código sin cambiar funcionalidad
- [ ] 🧪 **Tests** - agrega o corrige pruebas
- [ ] 🔧 **Infraestructura** - cambios en CI/CD, Docker o configuración

## 🔗 Issue relacionado

<!-- Vincula el issue que este PR resuelve.
     Usa "Closes #N" para cerrarlo automáticamente al hacer merge. -->

Closes #

## 🧩 ¿Qué cambiaste?

<!-- Lista los cambios concretos que hiciste. Sé específico/a.
     Ej:
     - Agrega función `validate_serial()` en `utils.py`
     - Actualiza el endpoint POST /billetes para usar la nueva validación
     - Agrega tests para los casos vacío, formato inválido y formato válido -->

- 
- 
- 

## 🧪 ¿Cómo probarlo?

<!-- Explica paso a paso cómo un revisor puede verificar que los cambios funcionan.
     Incluye comandos, datos de prueba o configuraciones necesarias. -->

```bash
# Ej: levantar el entorno
docker compose -f compose.dev.yml up -d

# Ej: correr los tests
pytest tests/test_billetes.py -v
```

## 🖼️ Capturas de pantalla (si aplica)

<!-- Si el cambio afecta la interfaz visual, muestra el antes y después. Si no aplica, puedes borrar esta sección. -->

| Antes | Después |
|-------|---------|
|       |         |

## ✅ Checklist

<!-- Revisa cada punto antes de marcar el PR como listo para revisión -->

- [ ] Mi código sigue los estándares del proyecto (PEP 8)
- [ ] Probé los cambios localmente y funcionan
- [ ] Agregué o actualicé tests para cubrir los cambios (si aplica)
- [ ] Actualicé la documentación relevante (README, docstrings, comentarios)
- [ ] No hay conflictos con la rama `main`
- [ ] El título del PR sigue el formato: `tipo: descripción breve` (ej. `feat: agregar validación de serie`)
- [ ] Vinculé el issue relacionado con `Closes #N`

## 💬 Notas para el revisor

<!-- ¿Hay algo específico en lo que quieres que el revisor se enfoque?
     ¿Alguna decisión de diseño que quieras explicar o discutir?
     ¿Algo que sabes que no está completo y planeas terminar? -->