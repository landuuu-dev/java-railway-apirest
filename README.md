# API Endpoints

## Endpoints disponibles

### Listar todos los productos

```http
GET https://java-railway-apirest-production-8375.up.railway.app/productos
```

**Descripción:** Recupera la lista de todos los productos disponibles.

---

### Obtener producto por ID

```http
GET https://java-railway-apirest-production-8375.up.railway.app/productos?id=2
```

**Parámetros:**
| Key | Value     | Descripción                  |
|-----|----------|------------------------------|
| id  | `2`   | |

**Descripción:** Recupera el producto con el id especificado si se encuentra disponible.

---

### Agregar productos

```http
POST https://java-railway-apirest-production-8375.up.railway.app/productos
```

**Cuerpo de la solicitud (JSON):**
```json
{
    "nombre": "Agenda sin fechas + calendario",
    "precio": "15.00",
    "descripcion": "Agenda tamaño A5 con 100 hojas"
}
```

**Descripción:** Crea un nuevo producto con los datos especificados.

---

### Actualizar producto

```http
PUT https://java-railway-apirest-production-8375.up.railway.app/productos?id=2
```

**Parámetros:**
| Key | Value     | Descripción                  |
|-----|----------|------------------------------|
| id  | `2`   |  |

**Cuerpo de la solicitud (JSON):**
```json
{
    "nombre": "Libreta",
    "precio": "5.00",
    "descripcion": "Libreta tamaño A5 con 100 hojas"
}
```

**Descripción:** Actualiza los detalles de un producto existente.

---

### Eliminar producto

```http
DELETE https://java-railway-apirest-production-8375.up.railway.app/productos?id=2
```

**Parámetros:**
| Key | Value     | Descripción                  |
|-----|----------|------------------------------|
| id  | `2`   | |

**Descripción:** Elimina un producto del sistema según el ID especificado.
