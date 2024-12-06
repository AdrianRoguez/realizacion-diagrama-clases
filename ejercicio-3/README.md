# Sala de lectura
```java
public class SalaDeLectura {
    private String nombreSala;
    private int capacidad;
    private Map<String, Miembro> reservas;

    // Constructor vacío
    public SalaDeLectura() {
        this.reservas = new HashMap<>();
    }

    // Constructor por defecto
    public SalaDeLectura(String nombreSala, int capacidad) {
        this.nombreSala = nombreSala;
        this.capacidad = capacidad;
        this.reservas = new HashMap<>();
    }

    // Getters y setters
    public String getNombreSala() {
        return nombreSala;
    }

    public void setNombreSala(String nombreSala) {
        this.nombreSala = nombreSala;
    }

    public int getCapacidad() {
        return capacidad;
    }

    public void setCapacidad(int capacidad) {
        this.capacidad = capacidad;
    }

    public Map<String, Miembro> getReservas() {
        return reservas;
    }

    // Métodos
    public void verificarDisponibilidad() {
    }

    public void reservarSala() {
    }
}
```
# Editorial
```java
public class Editorial {
    private String nombre;
    private String direccion;
    private String contacto;
    private List<Libro> librosPublicados;

    // Constructor vacío
    public Editorial() {
        this.librosPublicados = new ArrayList<>();
    }

    // Constructor por defecto
    public Editorial(String nombre, String direccion, String contacto) {
        this.nombre = nombre;
        this.direccion = direccion;
        this.contacto = contacto;
        this.librosPublicados = new ArrayList<>();
    }

    // Getters y setters
    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public String getDireccion() {
        return direccion;
    }

    public void setDireccion(String direccion) {
        this.direccion = direccion;
    }

    public String getContacto() {
        return contacto;
    }

    public void setContacto(String contacto) {
        this.contacto = contacto;
    }

    public List<Libro> getLibrosPublicados() {
        return librosPublicados;
    }

    // Métodos
    public void registrarEditorial() {
    }

    public void listarLibrosDeEditorial() {
    }

    public void agregarLibro() {
    }
}
```
