* **Autor del resumen:** Guiselle Tatiana Zambrano Penagos
* **Creation date:** 11 de Febrero de 2020

# Tasa de rendimiento - Throughput rate
La entrada y la salida suelen variar con el tiempo.

* **IN(t) =** Tasa de llegada/entrada de trabajos en el momento t.
* **OUT(t) =** Tasa de abandono/salida de trabajo en el momento t.
* **IN =** Velocidad de entrada promedio por unidad de tiempo.
* **OUT =** Velocidad de salida promedio por unidad de tiempo.

Un sistema estable debe tener **IN = OUT = $\lambda$**

* **$\lambda$ =** El flujo del proceso.
* **$\lambda$ =** Rendimiento del proceso (trabajos por unidad de tiempo).

# Trabajo en proceso - Work-in-process - WIP

* Trabajos que han ingresado al proceso, pero que aún no lo han dejado.
* Una tendencia duradera en la fabricación ha sido reducir el WIP, al reducir
el tamaño de los lotes.
	* La filosofía **JIT**.
	* Fuerza la reducción en tiempos y costos de instalación.
* **WIP =** Trabajo promedio en proceso a lo largo del tiempo.
* **WIP(t) =** Trabajo en proceso en el tiempo t.
	* WIP(t) incrementa cuando IN(t)) **>** OUT(t).
	* WIP(t) decrementa cuando IN(t)) **<** OUT(t).

# Ciclo de tiempo - CT

* **Ciclo de tiempo:** Diferencia entre el tiempo de inicio y finalización del
trabajo.
* **Formula Litte:** Relación general entre el promedio de WIP, el rendimiento
$\lambda$ y el ciclo de tiempo (CT)
	$$
		WIP = \lambda * CT
	$$
* Implicaciones, todo lo demás igual.
	* CT más corto $\Leftrightarrow$ WIP más bajo.
	* Si $\lambda$ aumenta $\Rightarrow$ para mantener WIP en los niveles 
	actuales, CT debe reducirse.

# Ejemplos
## Ejemplo 1

Un restaurante de comida rápida recibe en promedio 1200 clientes por día (entre 
las 10:00 y las 22:00). Durante las horas pico (12:00 - 15:00 y 18:00 - 21:00), 
el restaurante recibe alrededor de 900 clientes en total, y se pueden encontrar 
90 clientes en el restaurante (en promedio) al tiempo. En las horas no pico, el
restaurante recibe 300 clientes en total, y se pueden encontrar 30 clientes en 
el restaurante (en promedio) en un momento determinado.

1. ¿Cuál es el tiempo promedio que un cliente gasta en el restaurante durante las
horas pico?

1. ¿Cuál es el tiempo promedio que un cliente pasa en el restaurante durante el 
horario no pico?

### Solución
1. Hora pico 12:00 - 15:00, 18:00 - 21:00.
$$
\begin{split}
	&15:00 - 12:00 = 3hrs \hspace{1cm} 21:00 - 18:00 = 3 hrs \hspace{1cm} 6hrs\\
	&\lambda = \frac{\textrm{Trabajos}}{\textrm{Unidad de tiempo}} = 
	\frac{900clientes}{6hrs} = 150\\
	&\lambda = 150 \hspace{1cm} WIP = 90\\
	&WIP = \lambda * CT \hspace{1cm} 90 = 150 * CT \hspace{1cm} CT = 
	\frac{90}{150}\\
	&CT = 0,6hrs = 36 min
\end{split}
$$

1. Hora no pico 10:00-12:00, 15:00-18:00, 21:00-22:00.
$$
\begin{split}
	&10:00-12:00=2hrs \hspace{1cm} 15:00-18:00=2hrs \hspace{1cm} 
	21:00-22:00=2hrsi \hspace{1cm}6hrs\\
	&\lambda = \frac{\textrm{Trabajos}}{\textrm{Unidad de tiempo}} = 
	\frac{1200 - 900clientes}{6hrs} = \frac{300}{6}=50\\
	&\lambda = 50 \hspace{1cm} WIP = 30\\
	&WIP = \lambda * CT \hspace{1cm} 30 = 50 * CT \hspace{1cm} CT = 
	\frac{30}{50}\\
	&CT = 0,6hrs = 36 min
\end{split}
$$

## Ejemplo 2
