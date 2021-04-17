---
title: Resolviendo la Integral de la Curva de Bell
category: article
---

Quería hacer esta entrada para compartir una demostración super corta pero que me resultó batante útil para entender
el siguiente resultado:

$$ \int_{-\infty}^{\infty} e^{-x^2}dx = \sqrt{\pi}$$

La cual es la curva de Bell. Un poco contraituitivo, y al ver a 
<span>
$$ \pi $$
</span>

ahí, uno inmediatamente piensa que tiene que ver con círculos. Bueno, eso es en parte a dónde vamos.

Una manera de resolver esta integral requiere llevarla al terreno de las integrales dobles: si le sumamos una variable
nuestra expresión quedaría así:

$$ \iint_{plano-xy} e^{-(x^2 + y^2)}dxdy $$

Similar, pero no igual a la que teníamos originalmente. Sin embargo, si pasamos esta expresión a coordinadas polares,
obtenemos algo mucho más parecido:

$$ \int_{-\infty}^{\infty}\int_{0}^{2\pi}e^{-r^2}rd \theta dr $$

Como la integral es con respecto a
<span>$$\theta$$</span>, podemos quitar todo lo que contenga una
<span> $$r$$</span>, lo cual, en ese caso, es toda la función.

$$ \int_{0}^{\infty} e^{-r^2}dr \int_{0}^{2\pi}d\theta $$

Es trivial que la segunda integral da <span>$$2\pi$$</span>, por lo que tenemos:

$$\int_{0}^{\infty}(e^{-r^2}r)(2\pi)dr $$

$$2\pi\int_{0}^{\infty}e^{-r^2}rdr $$

Y hasta aquí el conocimiento de integrales dobles. Ahora tenemos una simple integral que vamos a
resolver usando el método de sustitución:

$$ u = -r^2$$

$$du = -2rdr $$

Insertamos nuestra sustitución en la ecuación:

$$ \int_{} e^{-r^2}rdr = \int_{}e^ur\frac{du}{-2r} $$

$$ = \int_{}e^u \frac{-1}{2}du $$

$$ = - \frac{1}{2}e^u $$

Reemplazamos el valor de <span> $$ u = -r^2 $$ </span>, y obtenemos que nuestra antiderivada
queda:

$$ \int_{} e^{-r^2}rdr = -\frac{1}{2}e^{-r^2} $$

Y fácilmente reemplazamos en nuestra integral original:

$$ 2 \pi \int_{0}^{\infty} e^{-r^2}rdr 
= 2 \pi  -\frac{1}{2}e^{-r^2}  \Bigg|_{\infty}^{0} $$

$$ = 2 \pi \bigg[ -\frac{1}{2}e^{-(\infty)^2} - \Big(-\frac{1}{2}e^{-0^2} \Big) \bigg] $$

$$ = 2 \pi \bigg[ -\frac{1}{2}(0) - \Big(-\frac{1}{2}(1) \Big) \bigg] $$

$$ = 2 \pi \frac{1}{2} $$

$$ = \pi $$

Una vez que hemos resuelto esta integral, podemos volver a nuestro problema original:

$$ C = \int_{-\infty}^{\infty} e^{-x^2}dx $$

Ahora podemos escribir nuestro resultado en términos de <span> $$ C $$</span>

$$ C = \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} e^{-(x^2 + y^2)}dx dy $$

$$ = \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} e^{-x^2}e^{-y^2}dx dy $$

$$ \int_{-\infty}^{\infty} e^{-y^2}Cdy $$

$$ C \int_{-\infty}^{\infty} e^{-y^2}dy $$

$$ = C^2 $$

Y como sabemos que:

$$ \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} e^{-(x^2 + y^2)}dxdy = C^2 = \pi $$

$$ C = \sqrt{\pi} $$

Entonces:

$$ C = \int_{-\infty}^{\infty} e^{-x^2}dx = \sqrt{\pi} $$

Este es un ejemplo de cómo un conocimento más genérico de un tema (en este caso, las integrales
dobles en el campo de la integración) nos pueden llevar a entender el origen de un resultado
que antes tomábamos como "absoluto", o que asumíamos que era cierto sin demostración.

:~)