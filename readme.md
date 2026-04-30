## **¿Qué es un Pull Request (PR)?**

Un **Pull Request (PR)** es una solicitud para integrar cambios de una rama (*branch*) a otra dentro de un repositorio, normalmente hacia la rama principal (main o develop).

Es una pieza clave en el flujo de trabajo con Git, ya que permite **revisar, discutir y validar cambios antes de incorporarlos al proyecto**.

---

## **¿Para qué sirve un Pull Request?**

### **1.Revisar código**

Permite que otras personas del equipo revisen los cambios antes de aceptarlos.

Esto ayuda a:

- Detectar errores
- Mejorar la calidad del código
- Compartir conocimiento entre el equipo

---

### **2.Facilitar la comunicación**

Dentro del PR se pueden dejar comentarios, sugerencias o preguntas sobre líneas específicas del código.

Es como tener una conversación directamente sobre el código.

---

### **3.Validar cambios antes de integrarlos**

Antes de hacer *merge*, el equipo puede:

- Ejecutar pruebas
- Verificar que todo funciona correctamente
- Asegurarse de que no se rompe nada existente

---

### **4.Mantener un historial claro**

Cada PR queda registrado, lo que permite:

- Entender por qué se hizo un cambio
- Revisar decisiones pasadas
- Tener trazabilidad del proyecto

---

### **5.Trabajar en equipo sin conflictos**

Cada persona trabaja en su propia rama y luego propone sus cambios mediante un PR, evitando modificar directamente la rama principal.

---

## **Flujo básico de un Pull Request**

1. Crear una nueva rama:

```
git checkout -b feature/nueva-funcionalidad
```

1. 
2. Hacer cambios y commits:

```
git add .
git commit -m "feat: agregar nueva funcionalidad"
```

1. 
2. Subir la rama al repositorio remoto:

```
git push origin feature/nueva-funcionalidad
```

1. 
2. Crear el Pull Request en GitHub/GitLab
3. Revisar comentarios y hacer cambios si es necesario
4. Hacer *merge* del PR 🎉

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