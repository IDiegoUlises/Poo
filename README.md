# Poo editar
El paradigma de programación orientada a objetos es una metodología especial de programación de software en la que un programa informático se diseña como la interrelación entre un conjunto de instancias conocidas como objetos. Dichos objetos son entidades que tienen un estado que está descrito por sus variables internas que se conocen como atributos o propiedades; y que tienen comportamientos que están plasmados en funciones o métodos que se utilizan para manipular las variables que describen el estado del objeto.


```c++
//Se crea la clase
class Alumno
{
    //Declaracion de los atributos
  private:
    int edad;
    String nombre;

    //Declracion de los metodos
  public:
    Alumno(String, int); //Constructor
    void estudiar(); //Los metodos son funciones
    void escuchar();

};

//El constructor sirve para iniciar los atributos de la clase
Alumno::Alumno(String _nombre, int _edad)
{
  nombre = _nombre;
  edad = _edad;
}

void Alumno::estudiar()
{
  Serial.println(nombre);
}

void Alumno::escuchar()
{
  Serial.println(edad);
}


void setup() 
{
  Serial.begin(9600);
}

void loop() {
  //Se crea el objeto
  Alumno a1 = Alumno("Diego", 19);
  Alumno a2 = Alumno("Messi", 20);

  a1.estudiar();
  a1.escuchar();

  a2.estudiar();
  a2.escuchar();

  delay(500);
}
```
