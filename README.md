#include <iostream>
using namespace std;
int main()
{
    int opcion, cantidad;
    float suma=0, precio, ingreso;
	do {
		cout << "MENU" << endl;
		cout << "1. Hamburguesa (3Bs)" << endl;
		cout << "2. Hamburguesa con queso (5Bs)" << endl;
		cout << "3. Papas fritas (2Bs)" << endl;
		cout << "4. Soda (2.5Bs)" << endl;
		cout << "0. Salir" << endl;
		cout << "Ingrese una opcion: " << endl;
		precio = 0;
		cin >> opcion;
		switch (opcion) {
		case 1: precio = 3;
			break;
		case 2: precio = 5;
			break;
		case 3: precio = 2;
			break;
		case 4: precio = 2.5;
			break;
		case 0: cout << "salir" << endl;
			break;
		default:
			cout << "Error" << endl;
		}
		if (precio>0) {
			cout << "Ingrese la cantidad: ";
			cin >> cantidad;
			ingreso = cantidad + precio;
			suma = suma + ingreso;
		}
} while (opcion != 0);//Do-while sale por falso
	cout << "El monto total a pagar es: " << suma; 
	return 0;
}
	cout << "El monto total a pagar es: " << suma; 
	return 0;
}
