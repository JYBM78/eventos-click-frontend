# 🎭 Eventos Click — Frontend

## 📌 Descripción

**eventos-click-frontend** es el proyecto **frontend** desarrollado en **Angular** para la plataforma de gestión y compra de entradas de eventos artísticos, deportivos y culturales.

Está diseñado para ser **modular, escalable y colaborativo**, permitiendo que varios desarrolladores trabajen simultáneamente mediante ramas en Git.

---

## 🛠 Tecnologías

- Angular (TypeScript)
- SCSS para estilos
- npm para gestión de dependencias
- Git + GitHub para control de versiones

---

## 📂 Estructura principal

```plaintext
src/                # Componentes, estilos y lógica principal
angular.json        # Configuración del workspace Angular
package.json        # Dependencias y scripts npm
package-lock.json   # Bloqueo de versiones de dependencias
README.md           # Documentación y guía de uso
.vscode/            # Configuraciones recomendadas para VSCode


🌿 Flujo de ramas

master → versión estable del proyecto (solo producción)

dev → integración de nuevas funcionalidades (rama de equipo)

yovany, daniela, camilo → ramas personales de desarrolladores

👉 Cada desarrollador trabaja en su rama personal y luego integra sus cambios en dev.
👉 master contiene únicamente versiones estables y probadas.

🚀 Primeros pasos para nuevos desarrolladores

1️⃣ Clonar el repositorio

git clone https://github.com/TU_USUARIO/eventos-click-frontend.git
cd eventos-click-frontend

2️⃣ Cambiar a tu rama personal

git checkout tu-rama-personal
git pull origin tu-rama-personal

(El administrador ya creó ramas personales: yovany, daniela, camilo).

3️⃣ Instalar dependencias

npm install

4️⃣ Levantar servidor Angular

npm start

La aplicación estará disponible en:
👉 http://localhost:4200

y se recarga automáticamente al modificar archivos fuente.

🔄 Flujo de trabajo recomendado
1. Crear o trabajar en tu rama personal

git checkout yovany   # ejemplo

2. Hacer cambios y commits claros

git add .
git commit -m "feat: agregar formulario de registro"

👉 Usa prefijos:

feat: nueva funcionalidad

fix: corrección de bug

chore: tareas varias

3. Subir cambios al remoto

git push origin yovany


📥 Integración de cambios
De rama personal → dev

Crear un Pull Request (PR) en GitHub.

Revisar y aprobar cambios.

Merge a dev.

De dev → master

Solo cuando dev esté estable y probada:

git checkout master
git pull origin master
git merge dev
git push origin master

👩‍💻 Flujo de trabajo detallado para desarrolladores
Ejemplo: Daniela

1️⃣ Preparación inicial

git clone https://github.com/TU_USUARIO/eventos-click-frontend.git
cd eventos-click-frontend
git checkout daniela
git pull origin daniela


2️⃣ Desarrollo en local

git add .
git commit -m "feat: agregar formulario de registro de eventos"


3️⃣ Subir cambios al remoto

git push origin daniela


4️⃣ Integración en dev

Opción A: Pull Request (PR) desde GitHub.

Opción B: Merge manual en local:

git checkout dev
git pull origin dev
git merge daniela
git push origin dev


5️⃣ De dev a master (solo cuando está probado y estable):

git checkout master
git pull origin master
git merge dev
git push origin master

🔹 Flujo recomendado para Yovany
git checkout dev
git pull origin dev
git checkout yovany
git merge dev
# resolver conflictos si hay
git add .
git commit -m "fix: resolver conflictos con dev"
git push origin yovany


👉 Ahora Yovany puede seguir trabajando en su rama personal con lo más reciente.

🔹 Resumen gráfico del flujo
Rama personal (ej: daniela, yovany) → dev → master


dev: integración y pruebas.

master: solo versiones estables de producción.

✅ Todos los desarrolladores trabajan alineados.
✅ dev siempre actualizado.
✅ Los conflictos se resuelven pronto y no se acumulan.

📏 Buenas prácticas

Trabajar siempre en ramas personales (nunca directo en master ni en dev).

Actualizar tu rama personal con dev antes de trabajar:

git checkout dev
git pull origin dev
git checkout tu-rama
git merge dev


Hacer commits frecuentes y claros.

Probar localmente antes de subir cambios.

Mantener package-lock.json versionado para consistencia en dependencias.

📚 Recursos adicionales

Angular CLI — Overview

Documentación oficial de Angular
```
