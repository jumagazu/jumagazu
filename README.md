# Juan Manuel García Zúñiga

**Systems Engineer · Cali, Colombia**

I build web systems that replace the spreadsheets and legacy software small
companies actually run on. Most of my work starts the same way: sitting with the
people who do the job, understanding the process they already have, and building
around it instead of asking them to change.

---

## Currently building

### TimpaTec — Clinical records for occupational audiometry

A platform for an audiology practice that performs annual hearing tests for
companies' employees. Replaces a third-party system that couldn't adapt to how
they work.

- Patient records, clinical history, audiometry capture and diagnosis
- Threshold comparison against each worker's baseline exam, with the audiogram
  rendered to clinical convention — inverted dB axis, circles for the right ear,
  crosses for the left
- Printable clinical report with the practice's own branding
- Consolidated Excel export that mirrors, column for column, the spreadsheet the
  practice already uses — so the system fits their process on day one

**Next.js 16 · React 19 · TypeScript · Tailwind 4 · PostgreSQL (Supabase) · Vercel**

Some decisions worth mentioning, because they show how I think about data that
matters:

- Row Level Security enabled from the first migration, not retrofitted
- Constraints enforced in the database rather than only in the UI — a baseline
  exam *cannot* belong to a different patient, because a composite foreign key
  makes it impossible
- Calculated values (age, tenure, threshold differences) derived at read time
  instead of stored, so they can never drift out of sync

### Tempofy — Ear training for DJ students

A mobile app for practising beatmatching and time recognition with Latin music,
aimed at DJ students in Latin America.

---

## Working with

TypeScript · React · Next.js · PostgreSQL · C# · PHP · Angular

---

## A note on the empty profile

Most of my recent work is client software built under commercial agreements, so
those repositories are private. That's the honest reason this profile looks
quieter than the work behind it.

I'm glad to walk through architecture decisions, show the systems running, or
share code samples on request.

---

<details>
<summary><b>Español</b></summary>

<br>

**Ingeniero de Sistemas · Cali, Colombia**

Construyo sistemas web que reemplazan las hojas de cálculo y el software heredado
con el que funcionan muchas empresas pequeñas. Casi siempre empiezo igual:
sentándome con quienes hacen el trabajo, entendiendo el proceso que ya tienen, y
construyendo alrededor de eso en vez de pedirles que lo cambien.

### TimpaTec — Historia clínica para audiometría ocupacional

Plataforma para un centro de audiología que hace las audiometrías anuales a los
empleados de empresas cliente. Reemplaza un sistema de terceros que no lograba
adaptarse a su forma de trabajar.

- Registro de pacientes, antecedentes, captura de la audiometría y diagnóstico
- Comparación de umbrales contra el examen base de cada trabajador, con el
  audiograma dibujado según la convención clínica: eje de decibeles invertido,
  círculos para el oído derecho, equis para el izquierdo
- Informe clínico imprimible con la identidad del centro
- Exportación consolidada a Excel que replica, columna por columna, la hoja que
  el centro ya utiliza

**Next.js 16 · React 19 · TypeScript · Tailwind 4 · PostgreSQL (Supabase) · Vercel**

Algunas decisiones que vale la pena mencionar, porque muestran cómo pienso los
datos que importan:

- Row Level Security activo desde la primera migración, no agregado después
- Restricciones garantizadas en la base de datos y no solo en la interfaz: un
  examen base **no puede** pertenecer a otro paciente, porque una clave foránea
  compuesta lo hace imposible
- Los valores calculados —edad, antigüedad, diferencias de umbrales— se derivan
  al leer en vez de guardarse, así nunca quedan desactualizados

### Tempofy — Entrenamiento auditivo para estudiantes de DJ

Aplicación móvil para practicar beatmatching y reconocimiento de tiempos con
música latina, pensada para estudiantes de DJ en Latinoamérica.

### Sobre el perfil vacío

La mayor parte de mi trabajo reciente es software de clientes bajo acuerdos
comerciales, así que esos repositorios son privados. Esa es la razón honesta de
que este perfil se vea más quieto que el trabajo que hay detrás.

Con gusto repaso decisiones de arquitectura, muestro los sistemas funcionando o
comparto fragmentos de código si hace falta.

</details>
