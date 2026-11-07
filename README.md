# FORM-FB-01 — Fichas bibliográficas: fundamentos de sistemas distribuidos y arquitecturas distribuidas

Aplicaciones Distribuidas (ISR-701) · Universidad Técnica Estatal de Quevedo · SPA 2026–2027

**Grupo CLM**

| Integrante | Fichas | Referencias | Declaración de IA |
|---|---|---|---|
| Castro Coello Mario Sebastián | `fichas/castro.tex` | `bib/castro.bib` | `declaracion-ia/castro.tex` |
| Loor Suárez Jordan Josué | `fichas/loor.tex` | `bib/loor.bib` | `declaracion-ia/loor.tex` |
| Mendoza Villarroel Elian Jossue | `fichas/mendoza.tex` | `bib/mendoza.bib` | `declaracion-ia/mendoza.tex` |

## Contenido del repositorio

| Ruta | Descripción |
|---|---|
| `main.tex` | Archivo principal: carátula, índice, fichas de cada integrante, declaración de IA y referencias |
| `fichas/` | Cinco fichas bibliográficas por integrante |
| `bib/` | Referencias de cada integrante (BibLaTeX, estilo IEEE) |
| `declaracion-ia/` | Declaración de uso de inteligencia artificial de cada integrante |
| `main.pdf` | Informe compilado |

## Compilación del informe

- **Compilador:** `pdflatex`
- **Bibliografía:** `biber` (paquete `biblatex` con estilo `ieee`)
- **Archivo principal:** `main.tex`
- **Distribución usada:** MiKTeX 26.5 en Windows

Orden de comandos, ejecutados desde la raíz del repositorio:

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

El resultado es `main.pdf`.

### Dependencias

Paquetes de LaTeX: `fontenc`, `inputenc`, `babel` (idioma `spanish`), `lmodern`, `microtype`,
`geometry`, `booktabs`, `tabularx`, `enumitem`, `csquotes`, `biblatex` con `biblatex-ieee`, y `hyperref`.
Además se necesita el programa `biber`. MiKTeX instala automáticamente los paquetes que falten; en TeX Live
vienen incluidos en el esquema completo (`scheme-full`).
