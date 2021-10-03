# Poo
Programacion orientada a objetos
El paradigma de programación orientada a objetos es una metodología especial de programación de software en la que un programa informático se diseña como la interrelación entre un conjunto de instancias conocidas como objetos. Dichos objetos son entidades que tienen un estado que está descrito por sus variables internas que se conocen como atributos o propiedades; y que tienen comportamientos que están plasmados en funciones o métodos que se utilizan para manipular las variables que describen el estado del objeto.


```c++
#include <iostream>

using namespace std;

//Definicion de clases
class Alumno{
	private: //declaracion de los atributos
		int edad;
		string nombre;
		
	public: //Declracion de los metodos
		Alumno(int,string); //Constructor
		void estudiar(); //Los metodos son funciones
		void escuchar();
		
};
//El constructor sirve para iniciar los atributos de la clase
Alumno::Alumno(int _edad,string _nombre)
{
	edad = _edad;
	nombre = _nombre;
}

//Implementacion de los metodos
void Alumno::estudiar()
{
	cout << "Mi nombre es " << nombre << " y estoy estudiando." << endl;
}

void Alumno::escuchar()
{
	cout << "Tengo " << edad << " de edad y ahora estoy escuchando al profesor " << endl;
}

int main()
{
	Alumno a1 = Alumno(19,"Diego");
	Alumno a2 = Alumno(20,"Juan");
	
	a1.estudiar();
	a1.escuchar();
	
	a2.estudiar();
	a2.escuchar();
}
```
