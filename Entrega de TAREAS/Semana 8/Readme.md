## Instancia de Autoevaluación: Entrega de tarea ##

En esta instancia de autoevaluación vamos a poner en juego todos los conocimientos que hemos recorrido juntos en esta clase.  Tendremos en cuenta los tipos de ejercicios que realizamos la teoría que leímos y los ejemplos que vimos en los diferentes recursos.

 
Trabajaremos con el dataset disponible en campus el cual contiene los siguientes datos sobre clientes:

1.               purchase_freq_month — frecuencia de compras por mes (escala baja a media).

2.              avg_basket_usd — ticket/promedio por compra en USD (escala media a alta).

3.              time_on_site_min — tiempo de permanencia en el sitio (minutos).

4.             discount_sensitivity — sensibilidad a descuentos (0 a 1).

5.             returns_rate — tasa de devoluciones (0 a 0.8 aprox.).

Pista: algunas variables deberían ser escaladas antes de aplicar K-Means.

Qué se quiere descubrir con K-Means

●                    Objetivo: identificar cuántos segmentos latentes de clientes existen a partir de sus comportamientos de compra y uso del sitio, sin etiquetas previas.

●                    Qué patrones buscar:

o        Grupos con frecuencia alta pero ticket bajo y alta sensibilidad a descuentos.

o        Grupos con frecuencia baja pero ticket alto y baja sensibilidad (compras esporádicas pero grandes).

o        Grupos con tiempo en sitio y tasa de devoluciones diferenciados (p. ej., exploran mucho y devuelven más vs. exploran poco y devuelven menos).

●                    Cómo validarlo:

o        Comparar k=2..6 usando método del codo para justificar qué valor de k es razonable.

o        Analizar los centroides por cluster para describir perfiles (p. ej., “Cluster 1: alta frecuencia + ticket medio + sensibilidad media, foco para promociones; Cluster 2: ticket alto + baja sensibilidad, foco en upselling premium”, etc.).

En esta instancia deberás compartir tu jupyter notebook en tu repositorio GIT.

Es importante tener en cuenta que para aprobar esta instancia deberás:

●               Entregar en tiempo y forma

●               Realizar un 60% de la actividad correctamente.

●               Cumplir con las consignas

●               Cumplir con el formato requerido.
