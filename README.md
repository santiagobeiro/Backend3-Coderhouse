# Backend3-Coderhouse – Entrega Final Backend

Este proyecto forma parte del curso de **Backend en Coderhouse**. Se trata de una plataforma para la adopción de mascotas con funcionalidades completas: carga de mascotas, gestión de usuarios, sistema de adopciones, autenticación, tests, documentación Swagger, logger y dockerización.

---

## 🚀 Tecnologías

- Node.js
- Express.js
- MongoDB + Mongoose
- Docker
- Mocha + Chai + Supertest
- Multer
- Winston
- Swagger

---

## 📦 Instalación

```bash
git clone https://github.com/santiagobeiro/adoptpet-backend.git
cd adoptpet-backend
npm install
```

---

## ⚙️ Variables de entorno
Crea un archivo .env con el siguiente contenido:
```js
PORT=8080
MONGO_URL=mongodb+srv://<usuario>:<contraseña>@<cluster>.mongodb.net/<nombreDB>
```

---

## 🧪 Tests
```bash
npm test
```
Incluye pruebas funcionales para:
- ✅ api/adoptions
- ✅ api/sessions(register, login, current)

---

## 📄 Documentación Swagger
Disponible en:
👉 [http://localhost:8080/api/docs](http://localhost:8080/api/docs)

---

## 🐳 Docker

**Construir la imagen:**
```bash
docker build -t adoptme-backend .
```

**Ejecutar el contenedor:**
```bash
docker build -t adoptme-backend .
```

---

## 📤 Imagen en DockerHub
[enlace 🔗](https://hub.docker.com/r/santibeiro/adoptme-backend)
```bash
docker pull santibeiro/adoptme-backend
docker run -d -p 8080:8080 santibeiro/adoptme-backend
```

---

## Estructura del proyecto
```arduino
src/
├── controllers/
├── dao/
├── dto/
├── models/
├── repository/
├── routes/
├── services/
├── utils/
├── public/
├── config/
├── middlewares/
└── app.js
```

---

## 🔐 Funcionalidades principales
- Registro y login de usuarios con JWT y cookies
- Carga de imágenes y documentos con Multer
- Logger con múltiples niveles usando Winston
- Documentación Swagger completa para endpoints
- Dockerfile para despliegue
- mocks.router.js bajo la ruta /api/mocks
