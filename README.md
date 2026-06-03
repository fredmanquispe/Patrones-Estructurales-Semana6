Práctica: Patrones de Diseño Estructurales

Escuela Profesional de Ingeniería de Sistemas - UNA
Nombre: Hanz Fredman Quispe Quispe
Curso: Lenguajes de Programación Orientada a Objetos II
Docente: Mg. Aldo Hernán Zanabria Gálvez

Trabajo de Investigación (Patrones Estructurales)

1. Aplicación de Composite en Qt y Java Swing

Tanto en el framework Qt (C++) como en la biblioteca Java Swing (Java), las interfaces gráficas se organizan internamente siguiendo de forma rigurosa el patrón Composite. La clase abstracta principal (Component en Swing o QWidget en Qt) sirve como la interfaz base compartida. Los elementos simples de interacción como botones o campos de texto actúan como componentes "hoja", mientras que contenedores complejos como paneles o ventanas funcionan como "compuestos" que almacenan colecciones de otros elementos hijos. Cuando el motor gráfico ejecuta la renderización mediante llamadas como paint() o update(), el contenedor delega de manera recursiva la acción a todos sus elementos, permitiendo tratar de forma idéntica a una ventana entera o a un solo botón.

2. Decorator en Flask (Python) para el Manejo de Rutas

En el microframework web Flask, el patrón Decorator se manifiesta de forma nativa a través de funciones envolventes precedidas por el operador arroba (@). Su aplicación abarca principalmente el mapeo dinámico de rutas y la inyección de pre-condiciones globales de seguridad. Al declarar una ruta mediante @app.route('/url'), el framework intercepta una función ordinaria de Python y le añade la capacidad de responder a peticiones HTTP sin alterar su código interno. De la misma manera, permite empaquetar de forma externa restricciones de acceso (como un decorador personalizado @login_required) para validar la autenticidad de las sesiones antes de ejecutar la lógica principal de la vista.
