## **¿Qué es y para qué sirve un Pull Request (PR)?**

Un **Pull Request (PR)** es una solicitud para integrar cambios de una rama (*branch*) a otra dentro de un repositorio, normalmente hacia la rama principal (main o develop). Permite **revisar, discutir y validar cambios antes de incorporarlos al proyecto**.


### **1.Revisar código**
Permite que otras personas del equipo revisen los cambios antes de aceptarlos.

Esto ayuda a:

- Detectar errores
- Mejorar la calidad del código
- Compartir conocimiento entre el equipo


### **2.Facilitar la comunicación**
Dentro del PR se pueden dejar comentarios, sugerencias o preguntas sobre líneas específicas del código.

Es como tener una conversación directamente sobre el código.


### **3.Validar cambios antes de integrarlos**
Antes de hacer *merge*, el equipo puede:

- Ejecutar pruebas
- Verificar que todo funciona correctamente
- Asegurarse de que no se rompe nada existente


### **4.Mantener un historial claro**
Cada PR queda registrado, lo que permite:

- Entender por qué se hizo un cambio
- Revisar decisiones pasadas
- Tener trazabilidad del proyecto


### **5.Trabajar en equipo sin conflictos**
Cada persona trabaja en su propia rama y luego propone sus cambios mediante un PR, evitando modificar directamente la rama principal.

---

## **Flujo básico de un Pull Request**

1. Crear una nueva rama:

```
git checkout -b feature/nueva-funcionalidad
```

2. Hacer cambios y commits:

```
git add .
git commit -m "feat: agregar nueva funcionalidad"
```

3. Subir la rama al repositorio remoto:

```
git push origin feature/nueva-funcionalidad
```
 
4. Crear el Pull Request en GitHub
5. Revisar comentarios y hacer cambios si es necesario
6. Hacer *merge* del PR 🎉

---

## **🧠 Buenas prácticas**

- Haz PRs pequeños y enfocados (más fáciles de revisar)
- Escribe títulos y descripciones claras
- Revisa tu propio código antes de pedir revisión
- Responde a los comentarios del equipo
- Evita hacer merge sin revisión (si trabajas en equipo)

---

## **📹 Video de referencia**

Para aprender más sobre Pull Requests enfocados en colaboraciones de respositorios públicos, revisa este video:

[![Ver video sobre Pull Requests](https://img.youtube.com/vi/BPns9r76vSI/0.jpg)](https://youtu.be/BPns9r76vSI?si=MNZzhvezaB8VcwRS)

[Enlace directo: https://youtu.be/BPns9r76vSI?si=MNZzhvezaB8VcwRS](https://youtu.be/BPns9r76vSI?si=MNZzhvezaB8VcwRS)

---

# **🧪 Taller PR con tu proyecto base**

## **🎯 Objetivo del ejercicio**

Cada alumna deberá:

- Crear una rama
- Modificar la UI (botón, estilos, texto, etc.)
- Subir cambios
- Crear un Pull Request

---

## **🧑‍🏫 Paso 0: Proyecto base (tú)**

Usas exactamente este código que ya tienes 👌

👉 Súbelo a GitHub como:

```
pr-workshop
```

---

## **👩‍💻 Paso 1: Clonar y crear rama**

Ellas:

```
git clone <repo-url>
cd pr-workshop
git checkout -b feature/nombre-alumna
```

---

## **🛠️ Paso 2: Cambios que pueden hacer (elige uno por alumna)**

Aquí está la clave: dales opciones para que no todas hagan lo mismo.

---

### **🟣 Opción 1: Agregar un botón**

Modificar el HTML:

```
<div class="container">
    <h1>Bienvenidos al Taller de Pull Request</h1>
    <p>Esta es una página básica de inicio para el workshop de pull requests</p>

    <button class="btn">Haz clic aquí</button>
</div>
```

Y en CSS:

```
.btn {
    margin-top: 20px;
    padding: 10px 20px;
    border: none;
    background-color: #667eea;
    color: white;
    border-radius: 5px;
    cursor: pointer;
}

.btn:hover {
    background-color: #5a67d8;
}
```

---

### **🎨 Opción 2: Cambiar el fondo**

Modificar:

```
body {
    background: linear-gradient(135deg, #ff9a9e 0%, #fad0c4 100%);
}
```

---

### **✏️ Opción 3: Cambiar textos**

```
<h1>Mi primer Pull Request 🚀</h1>
<p>Estoy aprendiendo a trabajar con ramas y PRs</p>
```

---

### **💅 Opción 4: Cambiar estilo del contenedor**

```
.container {
    background: #f9f9f9;
    border: 2px solid #667eea;
}
```

---

### **✨ Opción 5 (pro level): Animación**

```
.container {
    transition: transform 0.3s ease;
}

.container:hover {
    transform: scale(1.05);
}
```

---

## **💾 Paso 3: Commit y push**

```
git add .
git commit -m "feat: agregar botón / cambiar estilos / etc"
git push origin feature/nombre-alumna
```

---

## **🔀 Paso 4: Crear PR**

En GitHub:

- Click en **Compare & pull request**
- Base: main
- Compare: su rama

---

## **📝 Qué deben escribir en el PR**

Puedes pedirles esto:

```
## Cambios realizados
- Agregué un botón
- Añadí estilos al botón

## ¿Qué hace?
Permite interacción básica en la UI
```

---

## **👀 Paso 5: Review (tu momento estrella)**

Coméntales cosas como:

- “¿Este color tiene suficiente contraste?”
- “¿Podrías mejorar el nombre de la clase?”
- “¿Qué pasaría en móvil?”

👉 Esto conecta con UX/UI (te viene perfecto por tu perfil 😏)

---

## **🔁 Paso 6: Correcciones**

Ellas:

```
git add .
git commit -m "fix: mejorar estilos del botón"
git push
```

👉 Se actualiza el PR automáticamente

---

## **✅ Paso 7: Merge**

Tú haces click en:

👉 **Merge Pull Request**

---

## **🎉 Paso 8: Ver resultado**

Todas hacen:

```
git checkout main
git pull
```

👉 Ven cómo el proyecto ahora tiene TODOS los cambios combinados

---

## **🔥 Dinámica pro (muy recomendada)**

Haz esto:

- 2 alumnas cambian **el mismo CSS (background)**
- Generas conflicto 💥
- Lo resuelven contigo

👉 Esto les vuela la cabeza (aprenden muchísimo)