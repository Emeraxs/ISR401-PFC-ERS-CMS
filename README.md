# ISR401-PFC-ERS-CMS

Repositorio del equipo para la Práctica Experimental Unidad IV (PE4) de la
asignatura Ingeniería de Requisitos (ISR-401), UTEQ. Contiene la validación,
gestión del cambio y trazabilidad del ERS del Proyecto Fin de Curso
**FabroGym**.

## Sistema del PFC
FabroGym — sistema de gestión para gimnasio (clientes, membresías, pagos,
instructores, rutinas, asistencia, inventario).

## Integrantes
- Castro Bajaña Ariel Omar
- Mera Arias Erick Jhair
- Sánchez Centeno Roselyn Andreina

## Estructura de carpetas
```
01_ERS/            ERS_v1.5.4.pdf (base), ERS_v1.5.7.pdf (línea base PE4), fuentes .docx/.tex
02_Inspeccion/      Checklists (Anexo A), registro de defectos (Anexo B), métricas
03_CCB/             RFC-01, RFC-02, RFC-03 y Acta del CCB
04_Trazabilidad/    Matriz de trazabilidad, exportación CSV del backlog, capturas del tablero CASE
05_Informe/         Informe PE4 en LaTeX (.tex, .bib), figuras y PDF compilado
06_Evidencias/      Capturas de Git, fotos de la sesión de inspección, declaración de uso de IA
CHANGELOG.md        Historial de versiones del ERS
README.md           Este archivo
```

## Instrucciones de compilación del informe (05_Informe/)

El informe `PE4_U4_CASTRO_MERA_SANCHEZ.tex` se compila con **pdfLaTeX + BibTeX**
(estilo bibliográfico IEEE, `IEEEtran.bst`).

**Requisitos:**
- Distribución LaTeX: MiKTeX o TeX Live (2023 o superior).
- Paquetes: `geometry`, `babel` (spanish), `hyperref`, `booktabs`, `tabularx`,
  `array`, `longtable`, `graphicx`, `float`, `enumitem`, `IEEEtran` (para el
  estilo bibliográfico `IEEEtran.bst`). Con MiKTeX en modo "install packages
  on the fly" se resuelven automáticamente.

**Pasos:**
1. Clonar el repositorio:
   ```bash
   git clone https://github.com/Emeraxs/ISR401-PFC-ERS.git
   cd ISR401-PFC-ERS/05_Informe
   ```
2. Compilar (archivo principal: `PE4_U4_CASTRO_MERA_SANCHEZ.tex`):
   ```bash
   pdflatex PE4_U4_CASTRO_MERA_SANCHEZ.tex
   bibtex PE4_U4_CASTRO_MERA_SANCHEZ
   pdflatex PE4_U4_CASTRO_MERA_SANCHEZ.tex
   pdflatex PE4_U4_CASTRO_MERA_SANCHEZ.tex
   ```
   (se compila dos veces al final para resolver referencias cruzadas y la
   tabla de contenidos/citas).
3. El PDF resultante es `PE4_U4_CASTRO_MERA_SANCHEZ.pdf`, en la misma carpeta.

## Línea base actual
- Versión del ERS: **v1.5.9**
- Tag de Git: `baseline-v1.5.9`
- Ver `CHANGELOG.md` para el detalle de los cambios aplicados por cada RFC
  aprobado en el CCB.
