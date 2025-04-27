# Capítulo III: Requirements Specification

## 3.1. To-Be Scenario Mapping

A continuación se presenta la realizacion del To-Be Scenario Mapping por cada user persona.

Segmento Objetivo 1: Juan Pérez

<img src="/assets/c03/to-be-01.png">

<br>

Segmento Objetivo 2: María Lopez

<img src="/assets/c03/to-be-02.png">

<br>

## 3.2. User Stories

<table>
    <thead>
        <tr style="text-align:center">
            <th>ID</th>
            <th>Nombre</th>
            <th>Descripción</th>
            <th>Criterios de aceptación</th>
            <th>Épica</th>
        </tr>
    </thead>
    <tbody>
        <tr style="text-align:center">
            <td>HU01</td>
            <td>Registrar un vehículo</td>
            <td><strong>Como</strong> propietario, <strong>Quiero</strong> registrar un vehículo en la plataforma <strong>Para</strong> que los arrendatarios puedan alquilarlo.</td>
            <td>
                <h5>Escenario 01: Registro exitoso.</h5>
                <strong>Dado</strong> que el propietario desea registrar un vehículo.<br>
                <strong>Cuando</strong> ingresa los detalles requeridos (marca, modelo, año, precio, etc.).<br>
                <strong>Entonces</strong> el sistema guarda el vehículo y lo pone disponible Para ser alquilado.
                <h5>Escenario 02: Fallo en el registro.</h5>
                <strong>Dado</strong> que el propietario intenta registrar un vehículo.<br>
                <strong>Cuando</strong> falta información o hay datos incorrectos.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error y no permite completar el registro hasta que se corrijan los datos.
            </td>
            <td>EP01</td>
        </tr>
        <tr style="text-align:center">
            <td>HU02</td>
            <td>Buscar vehículos disponibles</td>
            <td><strong>Como</strong> arrendatario, <strong>Quiero</strong> buscar vehículos disponibles en la plataforma <strong>Para</strong> seleccionar el que mejor se ajuste a mis necesidades.</td>
            <td>
                <h5>Escenario 01: Búsqueda exitosa.</h5>
                <strong>Dado</strong> que el arrendatario desea buscar un vehículo.<br>
                <strong>Cuando</strong> ingresa criterios como ubicación, precio y tipo de vehículo.<br>
                <strong>Entonces</strong> el sistema muestra una lista de vehículos que cumplen con los criterios de búsqueda.
                <h5>Escenario 02: No hay vehículos disponibles.</h5>
                <strong>Dado</strong> que el arrendatario busca un vehículo.<br>
                <strong>Cuando</strong> no hay vehículos que cumplan con los criterios de búsqueda.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje indicando que no hay vehículos disponibles.
            </td>
            <td>EP02</td>
        </tr>
        <tr style="text-align:center">
            <td>HU03</td>
            <td>Filtrar vehículos por precio</td>
            <td><strong>Como</strong> arrendatario, <strong>Quiero</strong> filtrar los vehículos por precio <strong>Para</strong> encontrar uno que se ajuste a mi presupuesto.</td>
            <td>
                <h5>Escenario 01: Filtro aplicado correctamente.</h5>
                <strong>Dado</strong> que el arrendatario desea filtrar vehículos por precio.<br>
                <strong>Cuando</strong> selecciona un rango de precios.<br>
                <strong>Entonces</strong> el sistema muestra vehículos que estén dentro de ese rango.
                <h5>Escenario 02: No hay vehículos en el rango de precio.</h5>
                <strong>Dado</strong> que el arrendatario filtra por un rango de precio.<br>
                <strong>Cuando</strong> no hay vehículos que coincidan con el rango seleccionado.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje indicando que no hay vehículos disponibles en ese rango de precios.
            </td>
            <td>EP03</td>
        </tr>
        <tr style="text-align:center">
            <td>HU04</td>
            <td>Ver detalles de un vehículo</td>
            <td><strong>Como</strong> arrendatario, <strong>Quiero</strong> ver los detalles de un vehículo específico <strong>Para</strong> tomar una decisión informada sobre alquilarlo.</td>
            <td>
                <h5>Escenario 01: Detalles mostrados correctamente.</h5>
                <strong>Dado</strong> que el arrendatario desea ver los detalles de un vehículo.<br>
                <strong>Cuando</strong> selecciona un vehículo de la lista de resultados de búsqueda.<br>
                <strong>Entonces</strong> el sistema muestra los detalles del vehículo, incluyendo marca, modelo, año, precio y reseñas.
            </td>
            <td>EP04</td>
        </tr>
        <tr style="text-align:center">
            <td>HU05</td>
            <td>Agregar vehículo a favoritos</td>
            <td><strong>Como</strong> arrendatario, <strong>Quiero</strong> agregar vehículos a una lista de favoritos <strong>Para</strong> poder revisarlos más tarde.</td>
            <td>
                <h5>Escenario 01: Vehículo agregado a favoritos.</h5>
                <strong>Dado</strong> que el arrendatario encuentra un vehículo de su interés.<br>
                <strong>Cuando</strong> selecciona la opción de agregar a favoritos.<br>
                <strong>Entonces</strong> el sistema guarda el vehículo en la lista de favoritos del arrendatario.
                <h5>Escenario 02: Fallo en la adición a favoritos.</h5>
                <strong>Dado</strong> que el arrendatario intenta agregar un vehículo a favoritos.<br>
                <strong>Cuando</strong> el sistema presenta un error o no registra correctamente el favorito.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error y no guarda el vehículo como favorito.
            </td>
            <td>EP05</td>
        </tr>
        <tr style="text-align:center">
            <td>HU06</td>
            <td>Calificar un vehículo</td>
            <td><strong>Como</strong> arrendatario, <strong>Quiero</strong> calificar un vehículo después de haberlo alquilado<strong>Para</strong> compartir mi experiencia con otros usuarios.</td>
            <td>
                <h5>Escenario 01: Calificación exitosa.</h5>
                <strong>Dado</strong> que el arrendatario ha completado un alquiler.<br>
                <strong>Cuando</strong> ingresa una calificación y una reseña del vehículo.<br>
                <strong>Entonces</strong> el sistema guarda la calificación y la reseña, y la asocia con el vehículo en cuestión.
                <h5>Escenario 02: Fallo en la calificación.</h5>
                <strong>Dado</strong> que el arrendatario intenta calificar un vehículo.<br>
                <strong>Cuando</strong> el sistema presenta un error o no guarda correctamente la calificación.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error y no guarda la calificación.
            </td>
            <td>EP06</td>
        </tr>
        <tr style="text-align:center">
            <td>HU07</td>
            <td>Contactar al propietario</td>
            <td><strong>Como</strong> arrendatario, <strong>Quiero</strong> contactar al propietario de un vehículo <strong>Para</strong> hacerle preguntas o coordinar detalles del alquiler.</td>
            <td>
                <h5>Escenario 01: Contacto exitoso.</h5>
                <strong>Dado</strong> que el arrendatario desea hacer una consulta al propietario.<br>
                <strong>Cuando</strong> selecciona la opción de contactar propietario y envía un mensaje.<br>
                <strong>Entonces</strong> el sistema envía el mensaje al propietario y notifica al arrendatario que el mensaje fue enviado correctamente.
                <h5>Escenario 02: Fallo en el envío del mensaje.</h5>
                <strong>Dado</strong> que el arrendatario intenta contactar al propietario.<br>
                <strong>Cuando</strong> hay un error en el sistema.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error e informa al arrendatario que el mensaje no pudo ser enviado.
            </td>
            <td>EP07</td>
        </tr>
        <tr style="text-align:center">
            <td>HU08</td>
            <td>Reservar un vehículo</td>
            <td><strong>Como</strong> arrendatario, <strong>Quiero</strong> reservar un vehículo <strong>Para</strong> asegurar su disponibilidad en una fecha y hora específicas.</td>
            <td>
                <h5>Escenario 01: Reserva exitosa.</h5>
                <strong>Dado</strong> que el arrendatario ha seleccionado un
 devuelto el vehículo al propietario,<br>
                <strong>Cuando</strong> el sistema marca el alquiler como completado,<br>
                <strong>Entonces</strong> el sistema permite que ambas partes dejen una reseña sobre la experiencia de la transacción.
                <h5>Escenario 02: No se puede dejar reseña sin completar el alquiler.</h5>
                <strong>Dado</strong> que el arrendatario o el propietario intentan dejar una reseña,<br>
                <strong>Cuando</strong> el alquiler aún no ha sido marcado como completado,<br>
                <strong>Entonces</strong> el sistema no permite dejar la reseña hasta que el proceso de alquiler haya concluido.
            </td>
            <td>EP05</td>
        </tr>
        <tr style="text-align:center">
            <td>HU09</td>
            <td>Ver el historial de alquileres</td>
            <td><strong>Como</strong> arrendatario, <strong>deseo</strong> ver el historial de mis alquileres anteriores, <strong>Para</strong> poder llevar un control de estos.</td>
            <td>
                <h5>Escenario 01: Historial mostrado correctamente.</h5>
                <strong>Dado</strong> que el arrendatario desea ver el historial de sus alquileres.<br>
                <strong>Cuando</strong> accede a la sección de historial de alquileres.<br>
                <strong>Entonces</strong> el sistema muestra una lista de sus alquileres anteriores con detalles como fecha, vehículo alquilado y reseñas.
                <h5>Escenario 02: No hay alquileres anteriores.</h5>
                <strong>Dado</strong> que el arrendatario accede a la sección de historial de alquileres.<br>
                <strong>Cuando</strong> no ha realizado alquileres previos.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje indicando que no tiene historial de alquileres.
            </td>
            <td>EP09</td>
        </tr>
        <tr style="text-align:center">
            <td>HU10</td>
            <td>Administrar pagos</td>
            <td><strong>Como</strong> arrendatario, <strong>Quiero</strong> gestionar mis pagos <strong>Para</strong> poder completar las transacciones de alquiler.</td>
            <td>
                <h5>Escenario 01: Pago exitoso.</h5>
                <strong>Dado</strong> que el arrendatario debe realizar un pago.<br>
                <strong>Cuando</strong> ingresa la información de su tarjeta o cuenta de pago y autoriza la transacción.<br>
                <strong>Entonces</strong> el sistema procesa el pago y confirma la transacción al arrendatario.
                <h5>Escenario 02: Pago fallido.</h5>
                <strong>Dado</strong> que el arrendatario intenta realizar un pago.<br>
                <strong>Cuando</strong> la información de pago es incorrecta o la transacción no puede ser procesada.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error indicando que el pago no pudo ser completado y sugiere revisar la información de pago o intentar nuevamente.
            </td>
            <td>EP10</td>
        </tr>
        <tr style="text-align:center">
            <td>HU11</td>
            <td>Ver perfil de usuario</td>
            <td><strong>Como</strong> usuario, <strong>Quiero</strong> ver mi perfil con mi información personal y de alquileres <strong>Para</strong> poder confirmar que este correcta.</td>
            <td>
                <h5>Escenario 01: Perfil mostrado correctamente.</h5>
                <strong>Dado</strong> que el usuario desea ver su perfil.<br>
                <strong>Cuando</strong> accede a la sección de perfil.<br>
                <strong>Entonces</strong> el sistema muestra su información personal, detalles de sus vehículos (si es propietario) y su historial de alquileres.
                <h5>Escenario 02: Error en la carga del perfil.</h5>
                <strong>Dado</strong> que el usuario intenta acceder a su perfil.<br>
                <strong>Cuando</strong> ocurre un error en la carga de los datos.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error y no se carga la información del perfil.
            </td>
            <td>EP11</td>
        </tr>
        <tr style="text-align:center">
            <td>HU12</td>
            <td>Editar perfil de usuario</td>
            <td><strong>Como</strong> usuario, <strong>deseo</strong> editar la información de mi perfil <strong>Para</strong> mantenerla actualizada.</td>
            <td>
                <h5>Escenario 01: Edición exitosa del perfil.</h5>
                <strong>Dado</strong> que el usuario quiere editar su información personal.<br>
                <strong>Cuando</strong> cambia la información en los campos de edición del perfil (nombre, dirección, número de teléfono, etc.).<br>
                <strong>Entonces</strong> el sistema guarda los cambios y actualiza su perfil con la nueva información.
                <h5>Escenario 02: Error en la edición del perfil.</h5>
                <strong>Dado</strong> que el usuario intenta actualizar su información personal.<br>
                <strong>Cuando</strong> no proporciona datos válidos en los campos requeridos.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error y no permite guardar los cambios hasta que se corrijan los datos.
            </td>
            <td>EP12</td>
        </tr>
        <tr style="text-align:center">
            <td>HU13</td>
            <td>Gestionar vehículos alquilados</td>
            <td><strong>Como</strong> propietario, <strong>deseo</strong> gestionar los vehículos que he alquilado <strong>Para</strong> mantener control de las transacciones.</td>
            <td>
                <h5>Escenario 01: Gestión correcta de vehículos alquilados.</h5>
                <strong>Dado</strong> que el propietario ha alquilado uno de sus vehículos.<br>
                <strong>Cuando</strong> accede a la sección de "Mis Vehículos Alquilados".<br>
                <strong>Entonces</strong> el sistema muestra una lista de los vehículos alquilados y sus detalles (arrendatario, fecha de alquiler, duración, etc.).
                <h5>Escenario 02: No hay vehículos alquilados en el historial.</h5>
                <strong>Dado</strong> que el propietario intenta gestionar sus vehículos alquilados.<br>
                <strong>Cuando</strong> no ha alquilado vehículos en el pasado o actualmente.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje indicando que no tiene vehículos alquilados Para gestionar.
            </td>
            <td>EP13</td>
        </tr>
        <tr style="text-align:center">
            <td>HU14</td>
            <td>Recibir notificaciones de disponibilidad de vehículos</td>
            <td><strong>Como</strong> arrendatario, <strong>deseo</strong> recibir notificaciones <strong>Para</strong> poder enterarme cuando un vehículo que me interesa esté disponible.</td>
            <td>
                <h5>Escenario 01: Notificación exitosa.</h5>
                <strong>Dado</strong> que el arrendatario marca un vehículo como favorito,<br>
                <strong>Cuando</strong> el vehículo esté disponible Para alquiler nuevamente,<br>
                <strong>Entonces</strong> el sistema envía una notificación al arrendatario indicando la disponibilidad del vehículo.
                <h5>Escenario 02: Fallo en la notificación.</h5>
                <strong>Dado</strong> que el arrendatario intenta marcar un vehículo como favorito,<br>
                <strong>Cuando</strong> el sistema presenta un error o no registra correctamente el favorito,<br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error y no envía notificaciones.
            </td>
            <td>EP14</td>
        </tr>
        <tr style="text-align:center">
            <td>HU15</td>
            <td>Visualizar página informativa</td>
            <td><strong>Como</strong> usuario, <strong>deseo</strong> poder acceder a una pagina de la empresa <strong>Para</strong> poder enterarme del servicio que ofrecen.</td>
            <td>
                <h5>Escenario 01: Acceso página.</h5>
                <strong>Dado</strong> que el usuario ingresa al link de la pagina,<br>
                <strong>Cuando</strong> tiene necesidad de buscar un vehiculo,<br>
                <strong>Entonces</strong> la pagina se le muestra al usuario cuando este lo solicita.
                <h5>Escenario 02: Fallo en la pagina.</h5>
                <strong>Dado</strong> que el usuario ingresa al link de la pagina,<br>
                <strong>Cuando</strong> la pagina no se muestra por un error o no registra correctamente el favorito,<br>
                <strong>Entonces</strong> no se logra ingresar, no queremos eso.
            </td>
            <td>EP15</td>
        </tr>
        <tr style="text-align:center">
    <td>HU16</td>
    <td>Visualizar Contactos</td>
    <td><strong>Como</strong> usuario, <strong>deseo</strong> poder acceder a la información de contacto de la empresa en la landing page <strong>Para</strong> ponerme en contacto rápidamente si tengo preguntas o dudas.</td>
    <td>
        <h5>Escenario 01: Acceso a la información de contacto.</h5>
        <strong>Dado</strong> que el usuario navega por la landing page,<br>
        <strong>Cuando</strong> el usuario busca la sección de contacto,<br>
        <strong>Entonces</strong> la página debe mostrar claramente la información de contacto (teléfono, email, redes sociales, etc.) para que el usuario pueda comunicarse fácilmente.
        <h5>Escenario 02: Información de contacto no disponible.</h5>
        <strong>Dado</strong> que el usuario navega por la landing page,<br>
        <strong>Cuando</strong> no se muestra la sección de contacto o los datos están incorrectos,<br>
        <strong>Entonces</strong> el usuario no podrá comunicarse con la empresa, generando una mala experiencia.
    </td>
    <td>EP16</td>
</tr>

<tr style="text-align:center">
    <td>HU17</td>
    <td>Landing Page Intuitiva</td>
    <td><strong>Como</strong> usuario, <strong>deseo</strong> que la landing page sea intuitiva y fácil de usar <strong>Para</strong> poder encontrar rápidamente la información que busco y navegar sin problemas.</td>
    <td>
        <h5>Escenario 01: Navegación exitosa.</h5>
        <strong>Dado</strong> que el usuario accede a la landing page,<br>
        <strong>Cuando</strong> el diseño es intuitivo y las opciones de navegación son claras,<br>
        <strong>Entonces</strong> el usuario podrá encontrar fácilmente la información y explorar la página sin dificultades.
        <h5>Escenario 02: Navegación confusa.</h5>
        <strong>Dado</strong> que el usuario accede a la landing page,<br>
        <strong>Cuando</strong> la página tiene un diseño poco intuitivo o confuso,<br>
        <strong>Entonces</strong> el usuario tendrá dificultades para encontrar la información deseada, lo que puede generar frustración.
    </td>
    <td>EP17</td>
</tr>

<tr style="text-align:center">
    <td>HU18</td>
    <td>Landing Page Responsiva</td>
    <td><strong>Como</strong> usuario, <strong>deseo</strong> que la landing page sea responsiva y se adapte a diferentes dispositivos <strong>Para</strong> poder acceder a la información desde mi móvil, tablet o computadora sin problemas de visualización.</td>
    <td>
        <h5>Escenario 01: Página responsiva.</h5>
        <strong>Dado</strong> que el usuario accede a la landing page desde cualquier dispositivo,<br>
        <strong>Cuando</strong> la página está bien diseñada y se adapta automáticamente a diferentes tamaños de pantalla,<br>
        <strong>Entonces</strong> el usuario podrá visualizar correctamente toda la información y navegar sin inconvenientes.
        <h5>Escenario 02: Página no responsiva.</h5>
        <strong>Dado</strong> que el usuario accede a la landing page desde su móvil o tablet,<br>
        <strong>Cuando</strong> la página no está adaptada para dispositivos móviles,<br>
        <strong>Entonces</strong> el usuario tendrá problemas de visualización, lo que puede afectar la usabilidad.
    </td>
    <td>EP18</td>
</tr>

    </tbody>
</table>

## 3.3. Impact Mapping

Impact map de nuestros segmentos objetivos

<img src="/assets/c03/Impact Mapping.png">

## 3.4. Product Backlog
Utilizamos la escala de Fibonacci para la estimación de los Story Points.

<table>
    <thead>
        <tr>
            <th>Epic / Story ID</th>
            <th>Título</th>
            <th>Descripción</th>
            <th>Story Points (1/2/3/5/8)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>HU01</td>
            <td>Registrar cuenta</td>
            <td><strong>Como</strong> usuario, <strong>deseo</strong> crear una nueva cuenta para entrar a la plataforma.</td>
            <td>3</td>
        </tr>
        <tr>
            <td>HU04</td>
            <td>Verificación de identidad</td>
            <td><strong>Como</strong> propietario y arrendatario, <strong>deseo</strong> que la plataforma verifique la identidad de los usuarios para asegurar la confiabilidad.</td>
            <td>5</td>
        </tr>
        <tr>
            <td>HU06</td>
            <td>Publicar un vehículo para alquiler</td>
            <td><strong>Como</strong> propietario, <strong>deseo</strong> publicar mi vehículo para que pueda ser alquilado.</td>
            <td>3</td>
        </tr>
        <tr>
            <td>HU07</td>
            <td>Buscar vehículos disponibles</td>
            <td><strong>Como</strong> arrendatario, <strong>deseo</strong> buscar vehículos disponibles cerca de mi ubicación para alquilar.</td>
            <td>5</td>
        </tr>
        <tr>
            <td>HU08</td>
            <td>Reservar un vehículo</td>
            <td><strong>Como</strong> arrendatario, <strong>deseo</strong> reservar un vehículo para una fecha y hora específicas.</td>
            <td>5</td>
        </tr>
        <tr>
            <td>HU11</td>
            <td>Calcular tarifas de alquiler</td>
            <td><strong>Como</strong> usuario, <strong>deseo</strong> ver el costo total del alquiler antes de confirmar la reserva.</td>
            <td>5</td>
        </tr>
        <tr>
            <td>HU13</td>
            <td>Ver historial de alquileres</td>
            <td><strong>Como</strong> arrendatario, <strong>deseo</strong> ver el historial de mis alquileres anteriores para llevar un registro de mis transacciones.</td>
            <td>1</td>
        </tr>
        <tr>
            <td>HU14</td>
            <td>Recibir notificaciones de disponibilidad de vehículos</td>
            <td><strong>Como</strong> arrendatario, <strong>deseo</strong> recibir notificaciones cuando un vehículo que me interesa esté disponible.</td>
            <td>1</td>
        </tr>
    </tbody>
</table>
