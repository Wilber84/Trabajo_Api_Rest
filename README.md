# Trabajo_Api_Rest
Trabajo de api rest de Wilber Loaiza

# Mi API REST de Usuarios
## Instalación
```
git clone <url-del-repo>
cd mi-api
npm install
```
## Ejecución
```
node index.js
```
## Autenticación
Todas las peticiones requieren el header:
```
x-api-key: mi-clave-secreta-2024
```
## Endpoints
| Método | Ruta | Descripción |
|---------|-------------------|---------------------------|
| GET | /usuarios | Listar todos |
| GET | /usuarios/:id | Obtener uno por ID |
| POST | /usuarios | Crear usuario |
| PUT | /usuarios/:id | Actualizar usuario |
| DELETE | /usuarios/:id | Eliminar usuario |
| GET | /usuarios?rol=X | Filtrar por rol |


## Diferencia entre readFileSync y readFile

- readFileSync: lee archivos de forma síncrona, es decir, bloquea la ejecución del programa hasta que el archivo se carga completamente en memoria. Durante ese tiempo, el servidor no puede atender otras peticiones.

- readFile (asíncrono): lee archivos sin bloquear el hilo principal. Mientras el archivo se procesa, el servidor puede seguir atendiendo otras solicitudes, lo que mejora el rendimiento.

Se recomienda usar la versión asíncrona en entornos de producción, ya que permite manejar múltiples peticiones de manera más eficiente.
