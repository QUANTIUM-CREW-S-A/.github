# Cómo contribuir

Gracias por el interés en los proyectos de **QUANTIUM CREW, S.A.** Este documento fija las
convenciones que aplican a todos los repositorios de la organización.

## Antes de escribir código

1. Revise los issues abiertos; puede que el trabajo ya esté en curso.
2. Para un cambio grande, abra primero una **propuesta de mejora** y espere confirmación. Un
   pull request extenso sin acuerdo previo suele terminar rechazado, y no queremos hacerle
   perder el tiempo.
3. Para errores, use la plantilla de **reporte de error** con pasos reproducibles.

## Entorno de trabajo

```bash
git clone https://github.com/QUANTIUM-CREW-S-A/<repositorio>.git
cd <repositorio>
cp .env.example .env     # complete los valores; nunca los suba
npm install              # o el gestor que indique el README del proyecto
```

Cada repositorio manda sobre este documento en lo específico: lea siempre su `README.md`.

## Ramas

```
main                 siempre desplegable, protegida
feat/nombre-corto    una funcionalidad
fix/nombre-corto     una corrección
chore/nombre-corto   mantenimiento
docs/nombre-corto    documentación
```

Sin tildes, sin espacios y sin números de versión como nombre de rama. Una rama, un tema.

## Commits

Usamos [Conventional Commits](https://www.conventionalcommits.org/es/):

```
tipo(ámbito): descripción en minúscula, en imperativo, sin punto final

feat(facturas): exportar a CSV con plantilla personalizable
fix(auth): evitar que la sesión expire al refrescar
docs(readme): agregar instrucciones de Docker
```

Tipos admitidos: `feat`, `fix`, `docs`, `refactor`, `test`, `chore`, `perf`, `style`.

Convención de idioma: **código e identificadores en inglés, documentación y mensajes de
commit en español.** Lo importante es no mezclar dentro de un mismo repositorio.

## Pull requests

- Uno por tema, lo más pequeño que sea razonable.
- Título en formato Conventional Commits.
- Complete la plantilla: qué cambia, por qué y cómo se probó.
- `lint` y `build` en verde antes de pedir revisión.
- Capturas obligatorias si el cambio se ve en pantalla.
- Se fusiona con *squash*, y la rama se borra al fusionar.

## Estilo

- Respete el formateador y el linter configurados en el repositorio; no reformatee archivos
  ajenos al cambio.
- Nada de código comentado ni de `console.log` olvidados.
- Los textos visibles al usuario van en español, salvo que el proyecto indique otra cosa.

## Seguridad y datos

- **Nunca** suba `.env`, llaves, tokens, volcados de base de datos ni datos reales de
  clientes. Si algo se escapa, avise de inmediato: se rota la credencial antes de limpiar el
  historial.
- Si detecta una vulnerabilidad, no abra un issue: siga [`SECURITY.md`](SECURITY.md).

## Licencia

Al contribuir acepta que su aporte se distribuya bajo la licencia del repositorio (MIT, salvo
que se indique otra).

## Conducta

Participar implica aceptar el [Código de Conducta](CODE_OF_CONDUCT.md).
