# Integra el Script en el Head del Sitio Web
Este script te permite controlar la frecuencia y duración de visualización de anuncios en tu sitio web utilizando los atributos HTML **data-time-view** y **data-cookie-view**.

## Atributos Utilizados:
**data-time-view:** Define la duración en segundos que el anuncio estará visible antes de cerrarse automáticamente.

## Ejemplo data-time-view: 
**data-time-view="8"** (el anuncio se cerrará automáticamente después de 8 segundos de visualización).

**data-cookie-view**: Establece el intervalo mínimo en minutos para que el anuncio vuelva a mostrarse.

## Ejemplo data-cookie-view:
Para mostrar el anuncio cada 1 minuto: **data-cookie-view="1"**.

Para cargar el anuncio siempre que se cargue la página: **data-cookie-view="0"**.

## Modifica el script según tus necesidades:
Puedes ajustar **data-time-view** para cambiar la duración de visualización del anuncio según tus requisitos específicos.

Utiliza **data-cookie-view** para controlar con qué frecuencia se muestra el anuncio, cambiando el valor según la frecuencia deseada (en minutos).

# script
```
<div id="adklg" data-time-view="8" data-cookie-view="1" style="display: none;">
    <div class="content-cnjk">
        <p class="ad-t">This is an advertisement. Wait <span id="counter-ad"></span> seconds...</p>
        <!-- ads here -->

    </div>
</div>
<script src="https://cdn.jsdelivr.net/gh/eswhik/OverlayAd/app.js"></script>
```
