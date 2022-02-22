#include <iostream>
#include<string>
using namespace std;

int main()
{
    int menu = 0; {};
    int jmn;
    int numc;
    char nombrepaciente[100], tratamiento[100], descripcion[100];
    int hora;
    int minutos;
    int preciounitariotrat;
    int cantidad,b;
    int preciounitario;
    int total;
    int a;

        do
        {
            cout << "BIENVENIDO AL MENU DE OPCIONES, POR FAVOR ELIJA UNA DE LAS SIGUIENTES OPCIONES" << endl;
            cout << "1-Agendar cita" << endl;
            cout << "2-Modificar cita" << endl;
            cout << "3-Eliminar cita" << endl;
            cout << "4-Lista de citas vigentes" << endl;
            cout << "5-Limpiar pantalla" << endl;
            cout << "6-Salir" << endl;
            cin >> jmn;
            switch (jmn) //(preguntar por problema del char error)
            {
            case 1:
                do
                {
                    cout << "El numero de cita es" << endl << numc + 1 << endl;
                    cout << "Nombre del paciente" << endl;
                    cin.ignore();
                    cin.getline(cin, nombrepaciente); //Se utilizaron estas librerias para poder introducir el nombre sin problema alguno. 
                    cout << "Hora del tratamiento" << endl;
                    cin >> hora;
                    cin >> minutos;
                    cout << "Nombre del tratamiento" << endl;
                    cin >> tratamiento;
                    cout << "Anada una descripcion" << endl;
                    cin >> descripcion;
                    cout << "Precio unitario del tratamiento" << endl;
                    cin >> preciounitariotrat;
                    cout << "Cantidad del tratamiento" << endl;
                    cin >> cantidad;
                    cout << "Precio unitario" << endl;
                    cin >> preciounitario;
                    total = cantidad * preciounitario;
                    cout << "Total" << endl;
                    break;
                }
            case 2:
                break;
            case 3:
                break;
            case 4:
                break;
            case 5:
                break;
            case 6:
                exit(EXIT_FAILURE);
                break;

            }
            cout << "¿Desea volver al menu?" << endl;
            cout << "Presione 1-Salir 2-No salir" << endl;
            cin << b;
        } while (b==2)
        {

        }
        
        return 0;
    }
    
}
