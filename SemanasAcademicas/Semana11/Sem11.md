# Semana 11: Revisión de Laboratorio (Java + Spring Boot)

## 1. ¿Qué revisamos esta semana?
En esta semana se realizó la **revisión y análisis** de un laboratorio basado en **Java + Spring Boot**.  
El objetivo fue entender la estructura del proyecto, identificar cómo se organizan las capas (controlador, servicio, repositorio) y comprobar el funcionamiento de los endpoints (rutas) de la API.

![Estructura del proyecto](../img/img01sem11.png)

---

## 2. Estructura típica del proyecto Spring Boot
En el laboratorio se revisó cómo se organiza un backend profesional en Spring Boot, donde cada paquete cumple una función específica. Esto ayuda a mantener el código ordenado, escalable y fácil de mantener.

| Capa / Paquete      | Rol principal                                                  | Ejemplo |
|--------------------|----------------------------------------------------------------|---------|
| **Controller**      | Recibe solicitudes HTTP (GET/POST/PUT/DELETE) y devuelve respuesta (JSON). | `@RestController`, `@RequestMapping` |
| **Service**         | Contiene la lógica de negocio (validaciones, reglas, procesos). | `@Service` |
| **Repository**      | Acceso a datos (consultas, persistencia). Normalmente con JPA. | `@Repository`, `JpaRepository` |
| **Model / Entity**  | Representa la información del sistema (tablas / objetos de dominio). | `@Entity`, `@Table` |
| **Config**          | Configuraciones del sistema (CORS, seguridad, beans, etc.). | `@Configuration` |

---

## 3. Anotaciones clave que se identificaron
Durante la revisión se reforzó el uso de anotaciones para definir el comportamiento del framework, especialmente en controladores REST y en el manejo de dependencias.

| Anotación | ¿Para qué sirve? |
|-----------|-----------------|
| `@SpringBootApplication` | Clase principal que inicia el proyecto Spring Boot. |
| `@RestController` | Declara una clase como controlador REST (respuestas tipo JSON). |
| `@GetMapping`, `@PostMapping` | Define rutas HTTP por método (GET, POST, etc.). |
| `@Autowired` | Inyección de dependencias (conecta Controller → Service → Repository). |
| `@Entity` | Marca una clase como entidad de base de datos (ORM). |

![Endpoints en Postman](../img/img02sem11.png)

---

## 4. Flujo de una petición en la API (lo más importante)
Se revisó el recorrido completo que sigue una solicitud desde que sale del cliente (Postman / navegador) hasta que llega a la base de datos y regresa como respuesta:

- Cliente envía una solicitud HTTP a un endpoint.  
- El **Controller** recibe la ruta y valida parámetros.  
- El **Service** procesa reglas del negocio.  
- El **Repository** consulta o guarda datos.  
- Spring devuelve la respuesta en formato **JSON**.

### Ejemplo: Endpoint REST (estructura)
```java
@RestController
@RequestMapping("/api")
public class DocenteController {

  @GetMapping("/docentes")
  public List<Docente> listar() {
    return servicio.listar();
  }
}

