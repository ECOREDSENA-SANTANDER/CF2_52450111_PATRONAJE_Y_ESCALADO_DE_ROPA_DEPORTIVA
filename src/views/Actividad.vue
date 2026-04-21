<template lang="pug">
.curso-main-container.pb-3
        BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
        .container.tarjeta.tarjeta--blanca.p-4.p-md-5
        // Para cuestionario usar: ActividadController(:cuestionario="cuestionario") 
        // Para parrafo usar: ActividadController(:parrafo="parrafo")
        ActividadController(:cuestionario="cuestionario")
</template>

<script>
import ActividadController from '@ecored-sena/base-kit/plugin/components/actividad/ActividadController.vue'

export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    parrafo: {
      tema: 'Comprendiendo el diseño de presupuestos y estrategias de ahorro',
      titulo: 'Completar frases',
      introduccion:
        '<b> Objetivo:</b> identificar conceptos clave relacionados con el presupuesto personal, la cultura del ahorro y la planificación financiera.',
      instruccion:
        'Complete correctamente los enunciados con la palabra que falta según los contenidos estudiados en el componente formativo.',
      imagen: require('@/assets/actividad/imagen5.png'),
      barajarPreguntas: true,
      textos: [
        {
          id: 1,
          texto:
            'El [respuesta] personal es una herramienta que permite proyectar ingresos y egresos para mantener la estabilidad económica.',
          respuesta: 'presupuesto',
        },
        {
          id: 2,
          texto:
            'La constancia en el cumplimiento del presupuesto refleja un alto nivel de [respuesta] financiera.',
          respuesta: 'disciplina',
        },
        {
          id: 3,
          texto:
            'Ahorrar no es lo que sobra, sino lo que se [respuesta] guardar antes de gastar.',
          respuesta: 'planifica',
        },
        {
          id: 4,
          texto:
            'Un gasto innecesario que puede eliminarse sin afectar la calidad de vida básica se denomina gasto [respuesta].',
          respuesta: 'discrecional',
        },
        {
          id: 5,
          texto:
            'La cultura del ahorro promueve el uso responsable de los [respuesta] disponibles.',
          respuesta: 'recursos',
        },
        {
          id: 6,
          texto:
            'El estado de [respuesta] personales permite analizar la relación entre ingresos y egresos en un periodo determinado.',
          respuesta: 'resultados',
        },
        {
          id: 7,
          texto:
            'Cuando los ingresos son mayores que los egresos se generan una [respuesta] que puede destinarse al ahorro.',
          respuesta: 'utilidad',
        },
        {
          id: 8,
          texto:
            'Uno de los beneficios de ejecutar un presupuesto es la reducción del [respuesta] financiero.',
          respuesta: 'estrés',
        },
        {
          id: 9,
          texto:
            'Evitar gastos impulsivos y mantener límites presupuestales refleja [respuesta] financiera.',
          respuesta: 'disciplina',
        },
        {
          id: 10,
          texto:
            'Contar con un fondo de [respuesta] permite enfrentar gastos inesperados sin afectar el presupuesto.',
          respuesta: 'emergencia',
        },
      ],
    },
    cuestionario: {
      tema: 'Nombre del CF',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> Evaluar la comprensión y el uso adecuado de las herramientas básicas en la ventana <em>Board</em> del <em>software</em> EAGLE.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!..',
      titulo_reprobado: 'VUELVA A INTENTARLO..',
      preguntas: [
        {
          id: 1,
          texto:
            '¿Qué característica técnica distingue el trazado de prendas en tejido de punto respecto al patronaje en tejido plano?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'En el tejido de punto se incrementan las holguras para compensar la rigidez del material, mientras que en el tejido plano se eliminan completamente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'En el tejido de punto las holguras se reducen o eliminan según el porcentaje de elasticidad, aprovechando el comportamiento elástico del material. x',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Ambos tipos de tejido requieren holguras idénticas, ya que las variaciones dependen exclusivamente del diseño y no del material.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'En el tejido de punto se duplican los márgenes de costura para evitar el deshilachado, mientras que en el plano se trabaja sin márgenes.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de las diferencias técnicas entre los tipos de tejido y su implicación directa en las decisiones de trazado del patrón deportivo infantil.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 2,
          texto:
            '¿Cuál es la ventaja técnica principal de la manga ranglán en el vestuario deportivo infantil?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Permite reducir el consumo de tela al eliminar la pieza de manga, simplificando el despiece de la prenda.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Genera mayor estructura en el hombro y mejora la caída formal de la prenda en actividades de alta exigencia.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Elimina la costura de hombro convencional y la sisa tradicional, ampliando el rango de movimiento articular. x',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Facilita la incorporación de bolsillos funcionales en la zona de la sisa sin alterar la estructura del patrón base.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio de la construcción de la manga ranglán y su aplicación funcional en prendas deportivas infantiles.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 3,
          texto:
            'En el trazado de la sudadera de punto para el rango de 6 a 12 años, ¿qué función cumplen los puños y la pretina?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Son piezas decorativas que se agregan después del ensamble principal para mejorar la estética de la prenda.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Se trazan con medidas iguales al contorno corporal para garantizar que la prenda quede completamente ajustada.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Son elementos opcionales que solo se incluyen en diseños formales o de alta costura infantil.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Se trazan con medidas reducidas respecto al contorno corporal, aprovechando la elasticidad del tejido acanalado para garantizar el ajuste. x',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión del comportamiento técnico de los elementos de acabado en prendas de tejido de punto y su relación con la elasticidad del material.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 4,
          texto:
            '¿Qué variable técnica determina la disposición del patrón sobre la tela en prendas de tejido de punto?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'La dirección del mayor estiramiento del tejido, que generalmente se orienta en sentido horizontal. x',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'El color y el estampado del tejido, que condicionan la rotación de las piezas durante el trazado.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'El gramaje del tejido, que establece cuantas capas puede cortarse simultáneamente en producción.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'El tipo de costura aplicado en el ensamble, que define la orientación final de cada pieza sobre la tela.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia apropiación de los criterios técnicos que rigen la disposición del patrón en tejidos elásticos y su incidencia en el comportamiento de la prenda.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 5,
          texto:
            '¿Qué característica técnica diferencia el trazado de mallas y vestidos de baño respecto a otras prendas deportivas infantiles?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Se trazan exclusivamente en tejido plano con holguras amplias para facilitar el movimiento en actividades acuáticas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Requieren reducciones significativas en las medidas del patrón, dado que el tejido presenta elasticidad bidireccional. x',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Su construcción elimina el uso de piquetes y convenciones técnicas para simplificar el proceso de corte industrial.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Se elaboran con los mismos criterios de trazado de la sudadera, diferenciándose solo en el largo de la prenda.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio de las particularidades técnicas del patronaje en tejidos de elasticidad bidireccional y su aplicación en prendas deportivas especializadas.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 6,
          texto:
            '¿Cuál es el propósito técnico del escalado industrial en el proceso de producción de prendas de vestir?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Determinar el color y los acabados de las prendas para cada temporada de producción.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Registrar las instrucciones de costura y los tipos de puntadas requeridas en cada modelo.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Generar múltiples tallas a partir de un patrón base, manteniendo proporciones anatómicas y funcionalidad en cada una. x',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Calcular el consumo total de tela necesario para la producción de una colección completa.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión del concepto de escalado y su función esencial dentro del sistema de producción industrial de vestuario.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 7,
          texto:
            '¿Cuál de los siguientes principios técnicos del escalado garantiza que los ajustes entre tallas no generen desajustes entre sisas, mangas y cinturas?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Principio de proporcionalidad anatómica.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Principio de correspondencia dimensional. x',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Principio de funcionalidad ergonómica.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Principio de precisión técnica.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia apropiación de los principios metodológicos del escalado y la función específica que cada uno cumple en la coherencia dimensional del patrón.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 8,
          texto:
            '¿En qué contexto resulta más adecuado aplicar el escalado diferencial en prendas infantiles deportivas?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Cuando se requiere aplicar incrementos uniformes en todas las áreas del patrón para mantener la proporcionalidad general.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Cuando la serie de tallas es corta y los incrementos entre tallas son constantes y predecibles.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Cuando la prenda requiere ajustes puntuales en zonas específicas por exigencias ergonómicas o funcionales del movimiento. x',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Cuando el proceso de producción es manual y se necesita agilidad en la aplicación de los incrementos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los tipos de escalado y la pertinencia del método diferencial en prendas con requerimientos ergonómicos específicos.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 9,
          texto:
            '¿Qué caracteriza al método de escalado bibásico frente al monobásico?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'El bibásico utiliza una sola talla de referencia central para proyectar todos los incrementos de la serie.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'El bibásico toma dos tallas en los extremos del rango para calcular proporcionalmente los incrementos de las tallas intermedias. x',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'El bibásico aplica incrementos variables por zona del patrón, mientras el monobásico usa incrementos constantes en todo el molde.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'El bibásico se emplea exclusivamente en prendas de tejido de punto, mientras el monobásico se reserva para tejido plano.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio de los fundamentos metodológicos que distinguen los métodos de escalado y su aplicación en la graduación de series de tallas.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 10,
          texto:
            '¿En qué situaciones resulta especialmente adecuado el método de escalado monobásico?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'En rangos amplios de tallas con variaciones morfológicas complejas entre subetapas del desarrollo infantil.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'En prendas deportivas de alta especialización que requieren ajustes diferenciales en zonas de mayor exigencia física.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'En rangos de tallas reducidos con incrementos constantes y uniformes en todos los puntos de control. x',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Exclusivamente en procesos digitales donde el software calcula automáticamente los desplazamientos por coordenadas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los contextos de aplicación del escalado monobásico y su pertinencia en series de tallas con incrementos regulares.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 11,
          texto:
            '¿Qué función cumplen los ejes ortogonales en el método de escalado por coordenadas?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Definen la paleta cromática y la disposición de estampados sobre el patrón escalado.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Establecen el sistema de referencia geométrica desde el cual cada punto de control recibe valores de desplazamiento independientes en dos direcciones. x',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Determinan el margen de costura aplicable a cada talla de la serie según el tipo de tejido utilizado.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Indican la ubicación de los piquetes de ensamble en cada pieza del patrón graduado.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio del sistema de referencia geométrica del escalado por coordenadas y su función en la precisión de los desplazamientos por punto de control.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 12,
          texto:
            '¿Por qué el escalado por coordenadas es el método preferido para el trabajo con software de patronaje digital?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Porque elimina la necesidad de definir puntos de control, automatizando completamente el proceso sin intervención del patronista.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Porque trabaja exclusivamente con incrementos proporcionales que el software calcula a partir del cuadro de tallas importado.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Porque el sistema de ejes está integrado de forma nativa en el entorno digital, permitiendo ejecutar desplazamientos con mayor velocidad y precisión. x',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Porque reduce el número de piezas del patrón al fusionar automáticamente las zonas con incrementos similares.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de la articulación entre el método de escalado por coordenadas y las herramientas del entorno de patronaje digital.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 13,
          texto:
            '¿Qué representa el nido de escalado en el proceso de graduación de patrones?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'El archivo digital que almacena todas las reglas de escalado asignadas a cada punto de control del patrón.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'La tabla de incrementos que sintetiza los valores de desplazamiento por talla para cada punto del molde.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La superposición gráfica de todas las tallas de la serie sobre el patrón base, previa a la separación individual. x',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'El documento técnico que registra la secuencia de operaciones del proceso de escalado manual o digital.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia apropiación del concepto de nido de escalado y su función como etapa previa a la separación y marcación de tallas en producción industrial.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 14,
          texto:
            '¿Qué información mínima debe contener cada pieza de un patrón correctamente marcado para su uso en producción?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Nombre del patronista, tipo de fibra textil, temperatura de planchado y código cromático de los acabados.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Nombre de la pieza, talla, dirección del hilo, cantidad de veces a cortar, piquetes y referencia de la prenda. x',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Gama de mercado, universo de vestuario, temporada de uso, tipo de tejido y metraje total requerido por talla.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Tipo de máquina de costura, longitud de puntada, velocidad de avance y margen de costura por segmento.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia conocimiento de los elementos técnicos de marcación del patrón y su importancia en la trazabilidad del proceso de corte y confección.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 15,
          texto:
            '¿Por qué una separación y marcación deficientes del patrón generan impacto negativo en la producción industrial?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Porque impiden el registro del patrón en los sistemas de gestión documental del área de diseño.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Porque limitan la aplicación de los principios de proporcionalidad anatómica en las tallas extremas de la serie.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Porque generan errores en el tendido y el corte, con repercusiones directas sobre la calidad del producto terminado. x',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Porque dificultan la selección del método de escalado más adecuado para la siguiente temporada de producción.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión del impacto de la marcación técnica en la calidad del proceso productivo y la coherencia entre el patrón y la prenda final.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 16,
          texto:
            '¿Qué convención gráfica se recomienda para diferenciar visualmente las tallas dentro de un nido de escalado en trazado manual?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Aplicar diferentes tipos de línea (continua, discontinua, punteada) para cada talla de la serie. x',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Utilizar símbolos numéricos consecutivos en el centro de cada talla para facilitar su identificación.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Marcar únicamente la talla base con línea continua y dejar las demás tallas sin trazar hasta el corte.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Emplear exclusivamente el grosor de línea como diferenciador, prescindiendo del tipo de línea y el color.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia conocimiento de las convenciones gráficas aplicadas en la separación de tallas y su función en la legibilidad del patrón en producción.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 17,
          texto:
            '¿Cuál es el criterio técnico que debe verificarse en el nido de escalado antes de proceder al trazado definitivo de las tallas?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Que el porcentaje de aprovechamiento de tela sea superior al 85 % en todas las tallas de la serie.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Que los incrementos entre tallas consecutivas sean idénticos en todas las zonas del patrón.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Que las líneas de costura entre piezas complementarias mantengan continuidad en todas las tallas de la serie. x',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Que el patrón base coincida exactamente con las medidas del cuadro de tallas estandarizado nacional.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia apropiación de los criterios de verificación del nido de escalado y su relevancia para garantizar la coherencia dimensional entre piezas en toda la serie.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 18,
          texto:
            'En el patronaje de mallas deportivas infantiles, ¿qué zona del cuerpo presenta mayor complejidad técnica en el trazado y por qué?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'El escote, porque su curvatura debe adaptarse simultáneamente a las proporciones del cuello y los hombros del niño.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Las sisas, porque en tejidos de elasticidad bidireccional requieren amplitudes mayores que en tejidos convencionales.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'El tiro, porque integra medidas de profundidad, contornos y curvas específicas que deben ajustarse a las proporciones infantiles. x',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Los hombros, porque la reducción de holguras en tejido de punto altera significativamente la inclinación del patrón.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio de las particularidades técnicas del trazado de mallas infantiles y la complejidad geométrica de la zona del tiro en la construcción del patrón.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 19,
          texto:
            '¿Qué diferencia técnica existe entre el trazado de una malla completa y un vestido de baño de dos piezas en tejido de punto?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'La malla se construye en tejido plano y el vestido de dos piezas en tejido de punto con elasticidad bidireccional.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'En el vestido de dos piezas se elimina la entallada de cintura y el costado queda recto, mientras la malla conserva la curva de cintura. x',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'El vestido de dos piezas requiere holguras adicionales en toda la prenda, mientras la malla trabaja exclusivamente con reducciones.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'No existe diferencia estructural entre ambas prendas; la distinción es puramente estética y no afecta el patronaje.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de las diferencias constructivas entre tipologías de prendas acuáticas infantiles y su implicación técnica en el proceso de trazado.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
        {
          id: 20,
          texto:
            '¿Por qué el dominio del patronaje manual es condición indispensable para operar eficientemente un software de patronaje digital?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Porque el software solo funciona con patrones previamente trazados en papel que deben digitalizarse antes de su edición.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Porque las licencias de los programas de patronaje exigen certificación en métodos manuales para su activación.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Porque el conocimiento técnico del trazado manual, las fichas técnicas y los criterios de industrialización sustentan el uso eficiente de las herramientas digitales. x',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Porque el entorno digital reproduce exactamente los mismos pasos del trazado manual sin introducir ninguna variación metodológica.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de la relación entre el conocimiento técnico del patronaje manual y su articulación con las herramientas del entorno digital especializado.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con el patronaje infantil de prendas deportivas.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
