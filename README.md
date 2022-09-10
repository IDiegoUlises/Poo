# Poo
Es una metodologia especial de programacion en la que un programa informatico se diseña como la interrelacion entre un conjunto de instancias conocidas como objetos. Dichos objetos son entidades que tienen un estado que esta descrito por sus variables que se conocen como atributos o propiedades que tienen comportamientos que estan plasmados en metodos que se utilizan para manipular las variables que describen el estado del objeto.


```c++
//Se crea la clase
class Alumno
{
  //Declaracion de los atributos
  private:
    int edad;
    String nombre;

  //Declaracion de los metodos
  public:
    Alumno(String, int); //Constructor
    void estudiar(); //Declaracion de metodos
    void escuchar();

};

//Inicializa los atributos de la clase
Alumno::Alumno(String _nombre, int _edad)
{
  nombre = _nombre;
  edad = _edad;
}

//Define los metodos
void Alumno::estudiar()
{
  Serial.println(nombre);
}

//Define los metodos
void Alumno::escuchar()
{
  Serial.println(edad);
}


void setup()
{
  Serial.begin(9600); //Inicia el puerto serial
}

void loop()
{
  //Crea el objeto 1
  Alumno a1 = Alumno("Diego", 18);

  //Crea el objeto 2
  Alumno a2 = Alumno("Ulises", 20);

  //Llama los metodos del primer objeto
  a1.estudiar();
  a1.escuchar();

  //Llama los metodos del segundo objeto
  a2.estudiar();
  a2.escuchar();

  delay(5000); //Retardo de 5 segundos
}
```
