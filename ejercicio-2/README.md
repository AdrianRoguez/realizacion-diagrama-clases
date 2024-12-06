# Miembro
```java
// Clase Miembro
public class Miembro {
    private String nombre;
    private int idMiembro;
    private List<Prestamo> historialPrestamos;

    // Constructor vacío
    public Miembro() {
        this.historialPrestamos = new ArrayList<>();
    }

    // Constructor por defecto
    public Miembro(String nombre, int idMiembro) {
        this.nombre = nombre;
        this.idMiembro = idMiembro;
        this.historialPrestamos = new ArrayList<>();
    }

    // Getters y setters
    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public int getIdMiembro() {
        return idMiembro;
    }

    public void setIdMiembro(int idMiembro) {
        this.idMiembro = idMiembro;
    }

    public List<Prestamo> getHistorialPrestamos() {
        return historialPrestamos;
    }

    // Métodos
    public void registrarMiembro() {
    }

    public void verHistorial() {
    }
}
```
# Libro
```java
// Clase Libro
public class Libro {
    private String titulo;
    private String autor;
    private String isbn;
    private Categoria categoria;
    private boolean disponible;

    // Constructor vacío
    public Libro() {
    }

    // Constructor por defecto
    public Libro(String titulo, String autor, String isbn, Categoria categoria, boolean disponible) {
        this.titulo = titulo;
        this.autor = autor;
        this.isbn = isbn;
        this.categoria = categoria;
        this.disponible = disponible;
    }

    // Getters y setters
    public String getTitulo() {
        return titulo;
    }

    public void setTitulo(String titulo) {
        this.titulo = titulo;
    }

    public String getAutor() {
        return autor;
    }

    public void setAutor(String autor) {
        this.autor = autor;
    }

    public String getIsbn() {
        return isbn;
    }

    public void setIsbn(String isbn) {
        this.isbn = isbn;
    }

    public Categoria getCategoria() {
        return categoria;
    }

    public void setCategoria(Categoria categoria) {
        this.categoria = categoria;
    }

    // Métodos
    public void verificarDisponibilidad() {
    }

    public void asignarCategoría(Categoria categoria) {
    }
}
```
# Préstamo
```java
// Clase Préstamo
public class Prestamo {
    private Date fechaPrestamo;
    private Date fechaDevolucion;
    private Libro libro;
    private Miembro miembro;

    // Constructor vacío
    public Prestamo() {
    }

    // Constructor por defecto
    public Prestamo(Date fechaPrestamo, Date fechaDevolucion, Libro libro, Miembro miembro) {
        this.fechaPrestamo = fechaPrestamo;
        this.fechaDevolucion = fechaDevolucion;
        this.libro = libro;
        this.miembro = miembro;
    }

    // Getters y setters
    public Date getFechaPrestamo() {
        return fechaPrestamo;
    }

    public void setFechaPrestamo(Date fechaPrestamo) {
        this.fechaPrestamo = fechaPrestamo;
    }

    public Date getFechaDevolucion() {
        return fechaDevolucion;
    }

    public void setFechaDevolucion(Date fechaDevolucion) {
        this.fechaDevolucion = fechaDevolucion;
    }

    public Libro getLibro() {
        return libro;
    }

    public void setLibro(Libro libro) {
        this.libro = libro;
    }

    public Miembro getMiembro() {
        return miembro;
    }

    public void setMiembro(Miembro miembro) {
        this.miembro = miembro;
    }

    // Métodos
    public void calcularMultaPorRetraso() {
    }

    public void marcarComoDevuelto() {
    }
}
```
# Bibliotecario
```java
// Clase Bibliotecario
public class Bibliotecario {
    private String nombre;
    private int idEmpleado;

    // Constructor vacío
    public Bibliotecario() {
    }

    // Constructor por defecto
    public Bibliotecario(String nombre, int idEmpleado) {
        this.nombre = nombre;
        this.idEmpleado = idEmpleado;
    }

    // Getters y setters
    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public int getIdEmpleado() {
        return idEmpleado;
    }

    public void setIdEmpleado(int idEmpleado) {
        this.idEmpleado = idEmpleado;
    }

    // Métodos
    public void registrarLibros() {
    }

    public void gestionarPrestamos() {
    }
}
```
# Categoría
```java
public class Categoria {
    private String nombre;
    private String descripcion;
    private List<Libro> libros;

    // Constructor vacío
    public Categoria() {
        this.libros = new ArrayList<>();
    }

    // Constructor por defecto
    public Categoria(String nombre, String descripcion) {
        this.nombre = nombre;
        this.descripcion = descripcion;
        this.libros = new ArrayList<>();
    }

    // Getters y setters
    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public String getDescripcion() {
        return descripcion;
    }

    public void setDescripcion(String descripcion) {
        this.descripcion = descripcion;
    }

    public List<Libro> getLibros() {
        return libros;
    }

    // Métodos
    public void agregarCategoria(Libro libro) {
    }

    public void listarLibrosPorCategoria() {
    }
}
```
