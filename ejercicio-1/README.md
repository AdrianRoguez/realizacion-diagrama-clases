```java
// Clase Cliente
public class Cliente {
    private String nombre;
    private String numeroContacto;
    private String correoElectronico;

    // Constructor vacío
    public Cliente() {
    }

    // Constructor por defecto
    public Cliente(String nombre, String numeroContacto, String correoElectronico) {
        this.nombre = nombre;
        this.numeroContacto = numeroContacto;
        this.correoElectronico = correoElectronico;
    }

    // Getters y setters
    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public String getNumeroContacto() {
        return numeroContacto;
    }

    public void setNumeroContacto(String numeroContacto) {
        this.numeroContacto = numeroContacto;
    }

    public String getCorreoElectronico() {
        return correoElectronico;
    }

    public void setCorreoElectronico(String correoElectronico) {
        this.correoElectronico = correoElectronico;
    }

    // Métodos
    public void registrarCliente() {
    }

    public void obtenerInformacion() {
    }
}
```

```java
// Clase Reserva
public class Reserva {
    private Date fechaEntrada;
    private Date fechaSalida;
    private Cliente cliente;
    private Habitacion habitacion;

    // Constructor vacío
    public Reserva() {
    }

    // Constructor por defecto
    public Reserva(Date fechaEntrada, Date fechaSalida, Cliente cliente, Habitacion habitacion) {
        this.fechaEntrada = fechaEntrada;
        this.fechaSalida = fechaSalida;
        this.cliente = cliente;
        this.habitacion = habitacion;
    }

    // Getters y setters
    public Date getFechaEntrada() {
        return fechaEntrada;
    }

    public void setFechaEntrada(Date fechaEntrada) {
        this.fechaEntrada = fechaEntrada;
    }

    public Date getFechaSalida() {
        return fechaSalida;
    }

    public void setFechaSalida(Date fechaSalida) {
        this.fechaSalida = fechaSalida;
    }

    public Cliente getCliente() {
        return cliente;
    }

    public void setCliente(Cliente cliente) {
        this.cliente = cliente;
    }

    public Habitacion getHabitacion() {
        return habitacion;
    }

    public void setHabitacion(Habitacion habitacion) {
        this.habitacion = habitacion;
    }

    // Métodos
    public void calcularCostoTotal() {
    }

    public void confirmarReserva() {
    }
}
```

```java
// Clase Habitación
public class Habitacion {
    private int numeroHabitacion;
    private String tipoHabitacion; // Ejemplo: "individual", "doble"
    private double precioPorNoche;
    private boolean disponible;

    // Constructor vacío
    public Habitacion() {
    }

    // Constructor por defecto
    public Habitacion(int numeroHabitacion, String tipoHabitacion, double precioPorNoche, boolean disponible) {
        this.numeroHabitacion = numeroHabitacion;
        this.tipoHabitacion = tipoHabitacion;
        this.precioPorNoche = precioPorNoche;
        this.disponible = disponible;
    }

    // Getters y setters
    public int getNumeroHabitacion() {
        return numeroHabitacion;
    }

    public String getTipoHabitacion() {
        return tipoHabitacion;
    }

    public double getPrecioPorNoche() {
        return precioPorNoche;
    }

    public void setPrecioPorNoche(double precioPorNoche) {
        this.precioPorNoche = precioPorNoche;
    }

    // Métodos
    public void comprobarDisponibilidad() {
    }

    public void cambiarEstado() {
    }
}
```
