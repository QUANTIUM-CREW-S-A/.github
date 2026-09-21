# Política de seguridad

Aplica a todos los repositorios de **QUANTIUM CREW, S.A.**

## Cómo reportar una vulnerabilidad

**No abra un issue público.** Escriba a **sharkstar03@gmail.com** con el asunto
`[SEGURIDAD] <repositorio>` e incluya:

- El repositorio y la versión o commit afectados.
- Una descripción del problema y su impacto.
- Los pasos para reproducirlo, o una prueba de concepto mínima.
- Si aplica, una mitigación temporal.

También puede usar el aviso privado de GitHub (*Security → Report a vulnerability*) en los
repositorios donde esté habilitado.

## Qué puede esperar

| Etapa | Plazo objetivo |
| --- | --- |
| Acuse de recibo | 3 días hábiles |
| Evaluación inicial y severidad | 10 días hábiles |
| Corrección o plan de corrección | Según severidad, priorizando las críticas |

Pedimos no divulgar el hallazgo públicamente hasta que exista una corrección disponible.
Con gusto damos crédito a quien reporte, salvo que prefiera el anonimato.

## Versiones cubiertas

Se atiende la **rama `main`** y la última versión publicada de cada proyecto. Las versiones
anteriores no reciben parches salvo acuerdo específico.

## Manejo de secretos

En esta organización:

- Ningún archivo `.env` se versiona; se publica únicamente `.env.example` con los nombres de
  las variables y sin valores.
- Toda credencial expuesta se **rota primero** y se limpia del historial después.
- El escaneo de secretos con protección de push se habilita en los repositorios públicos.

Si encuentra una credencial expuesta en alguno de nuestros repositorios, avísenos de
inmediato por el correo de arriba; ese reporte tiene prioridad sobre cualquier otro.

## Fuera de alcance

Ataques de denegación de servicio, ingeniería social al personal, hallazgos generados
únicamente por escáneres automáticos sin impacto demostrado, y sistemas de terceros que no
operamos.
