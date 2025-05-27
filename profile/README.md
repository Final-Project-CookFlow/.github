# Documentación y metodologías

## Metodología GitFlow

La [Metodología GitFlow](https://github.com/Factoria-F5-dev/git-flow) es un modelo alternativo de creación de ramas en Git en el que se utilizan ramas de función y varias ramas principales.

![Esquema GitFlow](https://camo.githubusercontent.com/406e2c38505508de3f4ac0ad863de44ae618e25f70e5e7df014e44970ce1c11c/68747470733a2f2f7777772e7a75702e636f6d2e62722f77702d636f6e74656e742f75706c6f6164732f323032332f30332f696d616765312d322e706e67)

## 🚀 **Convención para un buen commit**  



### ✅ 1. Usa un prefijo para indicar el tipo de cambio realizado en el código:  

| **Prefijo**   | **Descripción** |
|--------------|----------------|
| `feat`       | ✨ Nueva funcionalidad |
| `fix`        | 🛠️ Corrección de un error |
| `refactor`   | 🔄 Mejora en el código sin cambiar su funcionalidad |
| `test`       | ✅ Adición o modificación de tests |
| `docs`       | 📖 Cambios en la documentación |
| `chore`      | 🔧 Tareas de mantenimiento (ej. actualización de dependencias) |
| `style`      | 🎨 Cambios en formato, indentación, espacios en blanco, etc. |

---

### ✅ 2. Incluye la clave del ticket y el número de la tarea (JIRA)  

Esto permite una mejor trazabilidad dentro del equipo y en herramientas de gestión de proyectos.

📌 **Ejemplo:**  

feat(KEY-3334): Adoption form validation

## ✅ 2. Emplea mensajes claros y concisos, preferiblemente en inglés. Es mejor usar el imperativo (como dando una orden)
