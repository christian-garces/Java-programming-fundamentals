Documentación del Proyecto Taller 1

1. Introducción
Este proyecto corresponde al Taller 1 de programación, donde se desarrollan ejercicios prácticos en Java para reforzar conceptos fundamentales como estructuras de control, funciones, modularidad y buenas prácticas de codificación.
El objetivo es mostrar un conjunto de soluciones organizadas y documentadas que sirvan como referencia para estudiantes y desarrolladores en formación.

2. Arquitectura del Proyecto
El repositorio sigue una estructura organizada por paquetes:
Taller1/
│── src/main/java/com/christian/taller1/
│   ├── ejercicios/     # Ejercicios individuales del taller
│   ├── utils/          # Funciones auxiliares y reutilizables
│   └── main/           # Clase principal para ejecutar ejemplos
│── test/               # Pruebas unitarias
│── docs/               # Documentación técnica y diagramas
│── README.md

3. Requisitos
- Java 11+
- Apache Maven
- JUnit para pruebas unitarias

4. Instalación y Ejecución
Clonar el repositorio
git clone https://github.com/christian-garces/Taller1.git
cd Taller1

Compilar y ejecutar
mvn clean install
mvn exec:java -Dexec.mainClass="com.christian.taller1.Main"

5. Ejemplos de ejercicios
Ejemplo: cálculo de factorial
public static int factorial(int n) {
    if (n <= 1) return 1;
    return n * factorial(n - 1);
}

Ejemplo: validación de número par
public static boolean esPar(int numero) {
    return numero % 2 == 0;
}

6. Pruebas
Ejecuta las pruebas unitarias con:
mvn test

7. Roadmap
- [ ] Añadir más ejercicios prácticos (recursividad, colecciones, manejo de archivos).
- [ ] Documentar cada ejercicio con explicación teórica.
- [ ] Implementar interfaz gráfica simple para ejecutar los ejercicios.
- [ ] Añadir ejemplos de integración con Docker para despliegue.

8. Licencia
Este proyecto está bajo la licencia MIT.
Puedes usarlo, modificarlo y distribuirlo libremente, siempre dando crédito al autor.
