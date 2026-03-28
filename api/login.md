# Login

Permite autenticar a un usuario en el sistema mediante correo y contraseña.

---

## Endpoint

POST /api/login

---

## Descripción

Este endpoint valida las credenciales del usuario y retorna un token de autenticación junto con los datos del usuario si las credenciales son correctas.

---

## Parámetros

| Campo    | Tipo   | Requerido | Descripción              |
|----------|--------|-----------|--------------------------|
| email    | string |    Sí     | Correo del usuario       |
| password | int    |    Sí     | Contraseña del usuario   |

---

## Respuesta exitosa

```json
{
  "token": "abc123xyz",
  "user": {
    "id": 1,
    "name": "Juan Pérez",
    "email": "juan@email.com"
  }
}
```

---

## Respuesta incorrecta

{
  "message": "Credenciales incorrectas"
}

---