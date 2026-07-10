# ChefLocal 🍳

Compra y vende comida a tus vecinos

## 🚀 Características

✅ **Registro de Usuarios** - Clientes y Chefs  
✅ **Autenticación JWT** - Tokens seguros  
✅ **Envío de Tokens** - A todos los usuarios  
✅ **Notificaciones en Tiempo Real** - Socket.IO  
✅ **Gestión de Órdenes** - Estado del pedido  
✅ **Dashboard Admin** - Estadísticas  

## 📦 Instalación

```bash
npm install
cp .env.example .env
# Editar .env con tus variables
npm run dev
```

## 🔗 API Endpoints

### Autenticación
- `POST /api/auth/register/client` - Registrar cliente
- `POST /api/auth/register/chef` - Registrar chef
- `POST /api/auth/login` - Login
- `POST /api/auth/verify-email` - Verificar email
- `POST /api/auth/send-tokens-all` - Enviar tokens a todos (Admin)

### Usuarios
- `GET /api/users/:id` - Obtener usuario

### Chefs
- `GET /api/chefs/nearby` - Chefs cercanos

### Platos
- `GET /api/dishes/chef/:chefId` - Platos del chef

### Órdenes
- `POST /api/orders` - Crear orden
- `GET /api/orders/user/:userId` - Órdenes del usuario

## 📧 Email
Configura tus credenciales de email en `.env`

## 🛠️ Tech Stack
- Node.js + Express
- MongoDB
- JWT
- Socket.IO
- Nodemailer
