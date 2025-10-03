#include <iostream>
using namespace std;

template <typename T>

Class Nodo{
   T dato;
   Nodo* next;

public;
  T getDato(){
     return this ->dato;
  }
  void setDato(T dato){
     this->dato = dato;
  }
  Nodo* getNext(){
     return this->next;
  }
  void setNext(Nodo* next){
     this->next = next;
  }
  Nodo(T dato, Nodo* next){
     this->dato = dato;
     this->next = next;
  }
  
};


//Función insertar al inicio

template <typename T>
void inserInicio(Nodo<T>** cabeza, T dato) {
    Nodo<T>* nuevo = new Nodo<T>(dato);
    nuevo->setNext(*cabeza);
    *cabeza = nuevo;
}
