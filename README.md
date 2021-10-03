# Poo
Programacion ortientada a objetos
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
