
    public static void main(String[] args) {
        Cliente cliente = new Cliente();
        System.out.println("DATOS DE CLIENTE");
        cliente.setEdad("37");
        cliente.setNombre("Bruno");
        cliente.setTelefono("65248892");
        cliente.setCredito(400);

        System.out.println(cliente.getNombre());
        System.out.println(cliente.getEdad());
        System.out.println(cliente.getTelefono());
        System.out.println("Credito: " + cliente.getCredito());

        Trabajador trabajador = new Trabajador();
        System.out.println("DATOS DE TRABAJADOR");
        trabajador.setNombre("Leo");
        trabajador.setEdad("25");
        trabajador.setTelefono("5566321");
        trabajador.setSalario(3500);

        System.out.println(trabajador.getNombre());
        System.out.println(trabajador.getEdad());
        System.out.println(trabajador.getTelefono());
        System.out.println("Salario: " + trabajador.getSalario());
    }
}
class Persona{
    String edad;
    String nombre;
    String telefono;
    public Persona(){
    }
    public String getEdad(){
        return "Edad: " + this.edad;
    }
    public void setEdad(String edad){
        this.edad = edad;
    }
    public String getNombre(){
        return "Nombre; " + this.nombre;
    }
    public void setNombre(String nombre){
        this.nombre = nombre;
    }
    public String getTelefono(){
        return "Telefono: " + this.telefono;
    }
    public void setTelefono(String telefono){
        this.telefono = telefono;
    }


}
class Cliente extends Persona{
    int credito;

    public Cliente(){
    }
    public int getCredito(){
        return this.credito;
    }
    public void setCredito(int credito){
        this.credito = credito;
    }
}
class Trabajador extends Persona{
    int salario;

    public Trabajador(){
    }
    public int getSalario(){
        return this.salario;
    }
