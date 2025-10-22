# COMPLETAR  
Comparando sus conocimientos antes de hacer la práctica con sus conocimientos después de hacer la tarea, explicar los principales aprendizajes logrados para beneficio de su formación profesional.  
Si solucionó un problema presentado al realizar la práctica también se debe documentar.


Primero aprendí sobre limitar recursos en Docker.
Prevención de abusos, que el contenedor no consuma muchos recursos porque afecta el rendimiento o a otros contenedores.

Aislamiento y seguridad, menciona que se debe aislar para evitar que el contenedor contagíe a otros.

Gestión eficiente de recursos, menciona que se debe dar los recursos necesarios a los contenedores.

Estabilidad y rendimientos, dice que si un contenedor tiene una gestion eficiente de recursos no habra problemas.

Cumplimiento de políticas, seguir las normativas para cumplir estándares de seguridad, rendimiento o costos.

Luego, se aprendió a limitar el uso de memoria y calcular la memoria swap máxima la cual es  "memoria swap máxima= memory swap- memoryu", se realizo el calculo del ejemplo en donde la respuesta salio "724 megabytes".

Tambien aprendí sobre los comandos para limitar el uso de procesador, y se realizo la consulta de ver el número de procesadores virtuales la cual es "docker info | grep(linux) find(windows) "CPU" ".

Luego aprendí sobre el Healthcheck que se menciona que son comandos para saber si funciona correctamente un contenedor, también se menciona que hay que poner "|| exit 1" para cuando se encuentre un fallo nos retorne un numero distino de 0, o sino docker lo puede malinterpretar el estado de salud del contenedor, se menciona los intervalos los cuales pueden estar en segundos, minutos, horas, días, para lo cual se debe tener en cuenta lo siguiente:

Frecuencia adecuada, menciona que debe ser frecuente para encontra el problema.

Tiempo suficiente para recuperarse, se entiende que debe haber un tiempo de recuperación despues de un chequeo, donde se recupere y poder ir al siguiente chequeo.

Considerar el tiempo de timeout, se menciona que el intervalo debe ser mayor que el tiempo de timeout.

Ajuste según las necesidades, tener en cuenta para que va hacer la aplicación para tener en cuenta la criticidad.

Luego se aprendió sobre los dockerfile, entendí que es un archivo el cual tiene instrucciones las cuales nos ayuda a crear una imagen que posteriormente podemos usar, dentro de este archivo se menciona las siguientes instrucciones:

FROM: imagen en la cual se va a basar.

RUN: ayuda a prepara la imagen.

COPY: copia arhivos o directorios desde la maquina host al sistema de archivos del contenedor.

ADD: copia archivos o directorios desde el sistema de archivos host al sistema de archivos del contenedor.

CMD: define el comando predeterminado a ejecutarse cuando se inicie el contenedor.

ENTRYPOINT: configura el comando o script cuando se inicia un contenedor basado en la imagen.

EXPOSE: nos dice por cual puerto el contenedor va a escuchar.

ENV: para definir variables de entorno.

VOLUME: para definir un punto de montaje.

Tambien se realizo el ejemplo del Dockerfile, el cual dio problemas en el update debido a que centos 7 ya no tenia mirrors activos confiables, al final se cambio para que vaya a un repositorio de CentOS Vault, y se pudo completar ese ejemplo. También se menciona las imágenes huérfanas,. las cuales son las imagenes que no tiene etiqueta y no estan asociadas a un contenedor.

Por ultimo, se aprendío sobre las políticas de reinicio, las cuales son reglas qué debe hacer Docker cuando un contenedor se detiene, entre las cuales tenemos no(no reinicia), always(siempre reinicia), unless-stopped(si se detiene manualmente no se reinicia) y on failure(solo reinici con código de error distinto de 0).





