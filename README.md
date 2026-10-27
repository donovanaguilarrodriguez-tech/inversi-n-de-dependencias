# inversi-n-de-dependencias
Se evita el acoplamiento directo entre la gestion y las notificaciones.
La clase AdmProducto es la clase principal de administracion y no depende directamente de como se mandan los avisos.
Las clases EnviarEmail y EnviarApp son los detalles concretos que ejecutan los envios.

AdmProducto interactua con los envios a traves de una abstraccion. Esto permite cambiar o agregar nuevos medios de notificacion sin tener que reescribir la logica principal del sistema.
