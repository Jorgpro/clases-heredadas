# clases-heredadas
public class Main{

   public static void main(String[] args) {
       Trabajador trabajador= new Trabajador();
       Cliente cliente=new Cliente();
       Persona persona= new Persona();
       
       persona.setNombre ("Jorge Zapata");
       String nombre =persona.getNombre();
       System.out.println(nombre);

       persona.setEdad(35);
       int edad=persona.getEdad();
       System.out.println(edad);

       persona.setTelefono(1156534122);
       int telefono =persona.getTelefono();
       System.out.println(telefono);
       
       


       cliente.setCredito(50000);
       int credito =cliente.getCredito();
       System.out.println(credito);
      
       trabajador.setSalario(688);
       int salario =trabajador.getSalario();
       System.out.println(salario);
 
}
}

   class Persona{

      private int edad;
      private int telefono;
      private String nombre;
  
   public void setEdad(int edad ){
      this.edad= edad;
   }
   public int getEdad(){
      return edad;
   }


   public void setNombre( String nombre){
      this.nombre = nombre;
   }
   public String getNombre(){
      return nombre ;
   }
   public void setTelefono(int telefono){
      this.telefono= telefono;
   }
   public int getTelefono(){
      return telefono;
}
}

   
class Cliente extends Persona{
private int credito;
     
   public void setCredito(int credito ){
      this.credito= credito;
   }
   public int getCredito(){
      return credito;
   } 
 
   
   
}
class Trabajador extends Persona{
 private int salario;
           
   public void setSalario(int salario ){
      this.salario= salario;
   }
   public int getSalario(){
      return salario;
   }      
}
