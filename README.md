# Orpheus

Aplicación Spring Boot con CRUD básico de usuarios.

## Stack

- Spring Boot (Spring MVC, Spring Data, Spring Security)
- Thymeleaf
- Base de datos relacional (JPA)

## Modelo `User`

| Campo | Tipo | Descripción |
| --- | --- | --- |
| `id` | Long | Identificador autogenerado |
| `name` | String | Nombre completo |
| `email` | String | Correo único |
| `password` | String | Contraseña cifrada |
| `createdAt` | Instant | Fecha de creación |

## Endpoints

| Método | Ruta | Descripción |
| --- | --- | --- |
| GET | `/users` | Lista todos los usuarios |
| GET | `/users/{id}` | Obtiene un usuario |
| POST | `/users` | Crea un usuario |
| PUT | `/users/{id}` | Actualiza un usuario |
| DELETE | `/users/{id}` | Elimina un usuario |

## Ejecución

```sh
./mvnw spring-boot:run
```

La aplicación queda disponible en `http://localhost:8080`.
