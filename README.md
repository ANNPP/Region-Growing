# Region-Growing
Este tutorial fue creado para probar la versión 1.7 de PCL en ROS Fuerte.
Dentro del programa hacen uso de la función con la que tienes problema loadPCDfile.
El problema es, efectivamente que la imagen que quieres ver no esta referencia debidamente. 
En este caso se creo otro archivo llamado "prueba" que contiene un frame para la orientación de la nube de puntos.
Tf es el paquete que permite referenciar todos los sistemas que integran el robot. Por cierto, esto es indispensable en navegación... 
Añade el ejecutable del archivo .cpp llamado "prueba" a tu CMakeLists (o al archivo dónde se agregan los ejecutables en esta versión de PCL) y corre tus programas junto con el ejecutable de "prueba".  
Cuando abras Rviz, en Global Options en "Fixed_Frame" eliges "base_link" como nuevo centro de gravedad del robot. 
Espero que te sirva de ayuda. 
