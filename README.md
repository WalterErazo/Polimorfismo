# Laboratorio 3: Polimorfismo

## Codigo de Laboratorio: 
### Main
ublic class Main {
    public static void main(String[] args){
           Shape a1, b1, c1;
     
     a1 = new Rectangle(10,10);
     System.out.println(a1.toString());
     
     b1 = new Triangle(10,4);
     System.out.println(b1.toString());
     
     c1 = new Rectangle (5,5);
     System.out.println(c1.toString());
    }
}

### Class Shape: 

public interface Shape {
    public double getArea();
    public String toString();
}


### Class Rectangule 
public class Rectangle implements Shape {
    
    private double width;
    private double length;
    
    public Rectangle(double width, double lenght){
        this.width = width;
        this.length = length;
        
    }
    
    
    
    public double getArea(){
        return this.width * this.length;
    }
    public String toString(){
        return "Rectangle[width"+ this.width
        +"length " + this.length
        + "area " + this.getArea() + "]"; 
    }
}


### Class Triangle: 

public class Triangle implements Shape {
    
    private double base; 
    private double height;
    
    public Triangle (double base , double height){
        this.base = base;
        this.height = height;
    }
    
    public double getArea(){
        
        return (base * height) / 2;
    }
    
    public String toString(){
        return "Triangle [ base" + this.base
        + "height" + this.height 
        +"Area " + this.getArea() + "]";
    }
}



## ¿Qué es interfaz?
Zona de comunicación o acción de un sistema sobre otro.

##¿Qué es una clase abstracta?
Una clase que declara la existentcia de métodos pero no implementacion dicho métodos.

##¿Qué diferencia hay entre herencia e interfaces?
Herencia es que clases hijas heredan propiedades como metodos, atributos y también pueden tener diferentes a las propedades de la clase padre.
Poliformismo es que se cumple varias cosas como entre ellas le contrato que tienen con la clase padre.



## ¿Cual es la diferencia entre pila, cola y lista?
### Lista:
  Es un TAD que nos permite almacenar datos de forma ordenada.
  
### Pila:
  Es una estructura de datos en la que el último elemento en entrar es el primero en salir. Y tiene acceso a la Pila
  
### Cola:  
  Es una estructura de datos el cual el último elemento en entrar es el primero en salir. Y tiene acceso final a la Lista.


