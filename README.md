#incluir<bits/stdc++.h>

class Persona {
private:
    std::string nombre;
    int edad;
    double altura;

public:
    // Constructor para inicializar los atributos
    Persona(std::string n, int e, double a) {
        nombre = n;
        edad = e;
        altura = a;
    }

    // Métodos para obtener el valor de los atributos (getters)
    std::string getNombre() {
        return nombre;
    }

    int getEdad() {
        return edad;
    }

    double getAltura() {
        return altura;
    }

    // Métodos para establecer el valor de los atributos (setters)
    void setNombre(std::string n) {
        nombre = n;
    }

    void setEdad(int e) {
        edad = e;
    }

    void setAltura(double a) {
        altura = a;
    }
};

int main() {
    // Crear una instancia de la clase Persona
    Persona persona("Juan", 30, 1.75);

    // Imprimir los atributos utilizando los métodos get
    std::cout << "Nombre: " << persona.getNombre() << std::endl;
    std::cout << "Edad: " << persona.getEdad() << " años" << std::endl;
    std::cout << "Altura: " << persona.getAltura() << " metros" << std::endl;

    // Modificar los atributos utilizando los métodos set
    persona.setNombre("María");
    persona.setEdad(25);
    persona.setAltura(1.60);

    // Imprimir los atributos actualizados
    std::cout << "Nombre: " << persona.getNombre() << std::endl;
    std::cout << "Edad: " << persona.getEdad() << " años" << std::endl;
    std::cout << "Altura: " << persona.getAltura() << " metros" << std::endl;

    return 0;
}
