% Finest Fitness 
% Ezequiel Marchena
% Curso 2018/19

# Descripción general del proyecto

Aplicación para la gestión de entrenadores, clases y clientes de un gimnasio por parte del administrador. Los clientes, una vez registrados, tienen acceso a la aplicación y pueden consultar las rutinas propuestas por el gimnasio, las suyas propias, solicitar un entrenador personal, etc. Los entrenadores también tendrán acceso a la app, y podrán ver las clases que imparten, los clientes a los que entrenan, etc. Todo esto en un calendario semanal/mensual fácil de entender.

## Funcionalidad principal de la aplicación

El administrador es quien da de alta a nuevos clientes y nuevos entrenadores, para que sólo los usuarios del gimnasio tengan acceso a la app.

**Los clientes cuando acceden a la app ven varias secciones:**

* **Rutinas:** _(Rutinas propias del gimnasio a las que todo cliente tiene acceso)_
    * Fuerza
    * Volumen
    * etc
* **Mis rutinas:** _(Rutinas creadas por el cliente y a las que sólo él tiene acceso)_
    * Rutina torso-piernas
    * Otra rutina
    * Otra más
* **Clases:** _(Calendario de clases con plazas limitadas a las que puede inscribirse)_
    * Ver todas
    * Spinning
    * Yoga
    * etc
* **Entrenadores:** _(Lista de los entrenadores que pueden solicitar como entrenador personal)_
    * Pepito Pérez
    * Juan Rodriguez
* **Perfil:** _(Perfil con los datos del cliente)_
    * Foto de perfil
    * Nombre
    * Email
    * Fecha de nacimiento
	* Peso
	* Altura
	* Horario
	* Teléfono
	* Monitor asignado

En el apartado ***Clases*** el cliente ve un calendario que puede ser semanal o mensual (ambas opciones disponibles), en el que se ve nombre de la clase, monitor y horario. El cliente puede clicar en la clase que le interese para poder inscribirse ocupando así una de las plazas. Una vez ocupadas todas las plazas, no podrán inscribirse más clientes.

En el apartado ***Entrenadores*** puede ver una lista de los entrenadores que tiene el gimnasio y acceso a parte de su perfil, donde verán las especialidades de ese entrenador y solicitar que los entrene. Dicha solicitud tiene que ser aceptada por el entrenador o el administrador.

**Los entrenadores cuando acceden a la app verían algo similar a lo siguiente:**

* **Mis clases:**
    * Todo: _(Calendario con todo: entrenamientos y clases)_
    * Entrenamientos: _(Lista con los entrenamientos: se muestra nombre del alumno junto a la rutina y la hora)_
        * Pablo López Full-body 12:15-13:45
        * etc
    * Clases: _(Lista de clases: Nombre de la clase, horario, número de alumnos inscritos y número de plazas)_
        * Spinning 15:00-15:45 13/20
	    * etc
* **Alumnos:** _(Mismo listado que en entrenamientos aunque con más opciones)_ 
	* Pablo López Full-body 12:15-13:45
* **Mis rutinas:** _(Mismo funcionamiento que las rutinas creadas por los clientes)_
* **Perfil:** _(Perfil del entrenador con sus datos)_
	* Foto de perfil
    * Nombre
    * Email
    * Fecha de nacimiento
	* Peso
	* Altura
	* Especialidad
	* Teléfono

El entrenador puede clicar en el nombre del alumno y verá parte de su perfil, así como en el nombre de la rutina para ver los ejercicios, series, repeticiones y descansos que la componen.
También puede clicar en el nombre de una clase para ver el calendario de esas clases.

El gimnasio cuenta con un horario para cada día de la semana, los clientes no podrán tener horarios de entrada fuera de los horarios del gimnasio, tampoco se podrán crear clases que empiecen o terminen fuera de dichos horarios. Los clientes no pueden inscribirse a una clase que empiece antes de su horario de entrada.

Un cliente puede pasar a ser entrenador y viceversa, sería el administrador quien realizaría esta acción.

Las rutinas generales son creadas por el administrador.

Un cliente no puede ser cliente y entrenador a la vez.

Un cliente no puede inscribirse a dos clases que coincidan en horario. Un cliente no puede inscribirse a una clase si ya tiene un entrenamiento (con el entrenador) asignado que coincida con la hora de la clase.

Un entrenador no puede impartir dos clases que coincidan en horario. Un entrenador no puede impartir una clase y entrenar a un alumno al mismo tiempo.

Las clases son creadas por el administrador, que es quien asigna al entrenador.

Cada cliente pagará una mensualidad en función de la tarifa seleccionada. Las tarifas dependen de factores como la edad y el horario.

La tarifa es elegida por el cliente, pero es aplicada por el administrador, para que un cliente pueda cambiar de tarifa, tiene que hablar con el administrador y es este quien se la cambia.

## Objetivos generales

* Gestionar los clientes.
* Gestionar los entrenadores.
* Gestionar las clases.
* Gestionar los entrenamientos
* Gestionar las rutinas.
* Gestionar los horarios.
* Gestionar las mensualidades.

# Elemento de innovación

Uso de Amazon S3 para el almacenamiento de imágenes.

Pasarela de pago mediante Paypal para pagar las mensualidades.
