# Thesis API

Permite gestionar las tesis del sistema.

---

## Listar tesis

**Endpoint**

`GET /api/thesis`

**Descripción**

Obtiene todas las tesis registradas.

**Respuesta**

```json
[
  {
    "id": 1,
    "title": "Sistema Web",
    "abstract": "Descripción...",
    "tutor": "Ing. Juan",
    "user": {},
    "category": {},
    "tags": [],
    "files": []
  }
]
```

---

## Ver una tesis

**Endpoint**

`GET /api/thesis/{id}`

**Descripción**

Obtiene una tesis específica por su ID.

**Ejemplo**

`GET /api/thesis/1`

---

## Buscar tesis

**Endpoint**

`GET /api/thesis/search/{search}`

**Descripción**

Busca tesis por coincidencia en el título.

**Ejemplo**

`GET /api/thesis/search/sistema`

---

## Crear tesis

**Endpoint**

`POST /api/thesis`

**Descripción**

Crea una nueva tesis.

**Body (JSON)**

```json
{
  "title": "Sistema Web",
  "abstract": "Descripción...",
  "tutor": "Ing. Juan",
  "repo_url": "https://github.com/test",
  "demo_url": "https://demo.com",
  "user_id": 1,
  "category_id": 1
}
```

---

## Actualizar tesis

**Endpoint**

`PUT /api/thesis/{id}`

**Descripción**

Actualiza una tesis existente.

**Ejemplo**

`PUT /api/thesis/1`

---

## Eliminar tesis

**Endpoint**

`DELETE /api/thesis/{id}`

**Descripción**

Elimina una tesis del sistema.

**Ejemplo**

`DELETE /api/thesis/1`

