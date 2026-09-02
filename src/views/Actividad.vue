<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <ActividadController :cuestionario="cuestionario"/>
  
  </template>

<script>
import ActividadController from '@ecored-sena/base-kit/plugin/components/actividad/ActividadController.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'Atención al cliente',
      titulo: 'Cuestionario',
      introduccion:
        '<b>Objetivo:</b> validar el conocimiento adquirido sobre la atención al cliente.',
      barajarPreguntas: false,
      preguntas: [
        {
          id: 1,
          texto: '¿Qué es la atención al cliente?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Un proceso de producción de bienes.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Conjunto de actividades destinadas a satisfacer las necesidades y expectativas de los clientes.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Una estrategia financiera.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Un método de control de inventarios.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 2,
          texto:
            '¿Cuál es una característica fundamental de la atención al cliente?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Desinterés por las necesidades del usuario.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Respuesta tardía a las solicitudes.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Amabilidad, respeto y disposición de ayuda.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Comunicación limitada.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 3,
          texto: '¿Cuál es la finalidad principal de la atención al cliente?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Incrementar los costos operativos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Reducir la interacción con el consumidor.',
              esCorrecta: false,
            },
            { id: 'c', texto: 'Eliminar la competencia.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Lograr la satisfacción y fidelización del cliente.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 4,
          texto: '¿Qué se entiende por satisfacción del cliente?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Grado en que las expectativas del cliente son cumplidas o superadas.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Número de productos vendidos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Cantidad de empleados de una empresa.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Nivel de inventario disponible.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 5,
          texto:
            '¿Para qué sirven las normas técnicas en la atención al cliente?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Para aumentar los precios.', esCorrecta: false },
            {
              id: 'b',
              texto:
                'Para establecer criterios de calidad en la prestación del servicio.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Para reducir la comunicación.',
              esCorrecta: false,
            },
            { id: 'd', texto: 'Para controlar las ventas.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 6,
          texto: '¿Qué es la fidelización del cliente?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Captar nuevos clientes exclusivamente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Reducir el número de compradores.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Lograr que los clientes mantengan una relación continua con la empresa.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Disminuir los servicios ofrecidos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 7,
          texto: '¿Qué beneficio aporta la fidelización de clientes?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Incrementa las reclamaciones.',
              esCorrecta: false,
            },
            { id: 'b', texto: 'Reduce la confianza.', esCorrecta: false },
            { id: 'c', texto: 'Disminuye las ventas.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Favorece la recompra y la lealtad hacia la empresa.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 8,
          texto: '¿Qué son los hallazgos en la atención al cliente?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Estrategias de mercadeo.', esCorrecta: false },
            {
              id: 'b',
              texto:
                'Resultados obtenidos del análisis de la atención y el servicio prestado.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Métodos de producción.', esCorrecta: false },
            { id: 'd', texto: 'Técnicas de distribución.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 9,
          texto: '¿Cuál es una acción de mejora derivada de los hallazgos?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Ignorar las sugerencias de los clientes.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Eliminar canales de atención.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Implementar cambios para corregir deficiencias identificadas.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Reducir la calidad del servicio.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 10,
          texto:
            '¿Cuál es el primer paso para gestionar adecuadamente una reclamación?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Descartar la queja.', esCorrecta: false },
            { id: 'b', texto: 'Justificar el error.', esCorrecta: false },
            {
              id: 'c',
              texto: 'Escuchar atentamente al cliente.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Suspender la comunicación.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 11,
          texto: '¿Qué son las relaciones con los clientes?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Interacciones que la empresa mantiene con los clientes antes, durante y después de la venta.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Procesos financieros internos.',
              esCorrecta: false,
            },
            { id: 'c', texto: 'Actividades de producción.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Estrategias de importación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 12,
          texto: '¿Qué función cumplen los protocolos de atención?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Limitar la comunicación.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Aumentar la complejidad de los procesos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Establecer procedimientos estandarizados para atender a los clientes.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Controlar la competencia.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 13,
          texto: '¿Por qué son importantes las relaciones con los clientes?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Porque reemplazan la publicidad.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Porque eliminan los costos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Porque sustituyen la calidad del producto.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Porque fortalecen la confianza y la permanencia del cliente.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 14,
          texto: '¿Qué es un manual de servicio al cliente?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Un informe financiero.', esCorrecta: false },
            {
              id: 'b',
              texto:
                'Documento que reúne políticas, procedimientos y estándares de atención.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Un catálogo de productos.', esCorrecta: false },
            { id: 'd', texto: 'Un contrato comercial.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 15,
          texto: '¿Qué es el ciclo del servicio?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Un proceso de fabricación.', esCorrecta: false },
            { id: 'b', texto: 'Una estrategia de ventas.', esCorrecta: false },
            {
              id: 'c',
              texto:
                'Secuencia de interacciones entre el cliente y la empresa durante la prestación del servicio.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Un sistema contable.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 16,
          texto: '¿Por qué es importante medir el servicio?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Para aumentar los costos.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Para reducir la participación del cliente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Para evaluar la calidad e identificar oportunidades de mejora.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Para limitar la retroalimentación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 17,
          texto: '¿Qué es un momento de verdad?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Una estrategia publicitaria.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Situación en la que el cliente interactúa con la empresa y forma una percepción del servicio.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Un proceso de facturación.', esCorrecta: false },
            { id: 'd', texto: 'Un tipo de negociación.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 18,
          texto: '¿Cuál es un elemento de los momentos de verdad?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'El inventario físico.', esCorrecta: false },
            { id: 'b', texto: 'La producción industrial.', esCorrecta: false },
            {
              id: 'c',
              texto: 'El contacto directo entre cliente y empresa.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'La contabilidad.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 19,
          texto: '¿Qué es el triángulo del servicio?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Una estrategia de publicidad digital.',
              esCorrecta: false,
            },
            { id: 'b', texto: 'Un modelo de ventas.', esCorrecta: false },
            {
              id: 'c',
              texto: 'Un sistema de distribución.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Modelo que integra cliente, personal y estrategia de servicio para garantizar calidad.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
        {
          id: 20,
          texto: '¿Qué es la trazabilidad en la atención al cliente?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La publicidad de productos.',
              esCorrecta: false,
            },
            { id: 'b', texto: 'El proceso de venta.', esCorrecta: false },
            {
              id: 'c',
              texto:
                'La capacidad de seguir y registrar cada interacción o proceso relacionado con el cliente.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'La clasificación de productos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la atención al cliente.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo atención al cliente.',
        },
      ],
      mensaje_final_aprobado:
        'Ha superado la actividad y demuestra sólidos conocimientos sobre la atención al cliente.',
      mensaje_final_reprobado:
        'No ha superado la actividad. Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
