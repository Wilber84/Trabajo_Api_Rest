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

- readFileSync: detiene la ejecución del programa hasta que el archivo se carga por completo en memoria.
- readFile (async): inicia la lectura y libera el bucle de eventos, permitiendo gestionar otras peticiones mientras el sistema de archivos trabaja.

Serecomienda usar la versión asíncrona.
