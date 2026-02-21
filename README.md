# vector-stats
Basic implementation of arrays in C++ for processing numerical data and calculating simple statistics.
#include <iostream>
using namespace std;

int main() {
    const int TAM = 5;
    int numeros[TAM];
    int suma = 0;
    float promedio;

    cout << "Ingrese 5 numeros:" << endl;

    for(int i = 0; i < TAM; i++) {
        cout << "Numero " << i + 1 << ": ";
        cin >> numeros[i];
        suma += numeros[i];
    }

    promedio = suma / (float)TAM;

    cout << "\nNumeros ingresados: ";
    for(int i = 0; i < TAM; i++) {
        cout << numeros[i] << " ";
    }

    cout << "\nSuma total: " << suma << endl;
    cout << "Promedio: " << promedio << endl;

    return 0;
}
