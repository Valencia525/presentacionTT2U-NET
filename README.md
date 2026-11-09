# Presentación Trabajo Terminal II: Decodificación ECoG con U-Net 1D y Optuna TPE

Repositorio oficial con los archivos fuente en **LaTeX Beamer** de la presentación de defensa del **Trabajo Terminal II (TT 2026-B145)**.

---

## 📋 Información del Proyecto

- **Institución:** Instituto Politécnico Nacional (IPN)
- **Unidad Académica:** Escuela Superior de Cómputo (ESCOM)
- **Programa Académico:** Ingeniería en Inteligencia Artificial
- **Registro de Trabajo Terminal:** TT 2026-B145
- **Título del Trabajo:** *Optimización bayesiana de redes neuronales para la decodificación de movimientos de los dedos a partir de señales electrocorticográficas*

### Autores
- **Saul Rodas Bautista**
- **Joel Valencia San Roman**

### Directores
- **Dra. Miriam Pescador Rojas**
- **M.C. Miguel Abel León Hernández**

---

## 🗂️ Estructura del Repositorio

```text
├── .vscode/               # Configuración de compilación para VS Code (LaTeX Workshop)
├── imgs/                  # Imágenes, diagramas de arquitectura y gráficas de resultados
├── slides/                # Módulos de diapositivas en LaTeX
│   ├── 01_contexto_problema.tex      # Portada, contexto, objetivos y cronograma
│   ├── 02_datos_preprocesamiento.tex # Preprocesamiento y análisis espectral
│   ├── 03_arquitectura_tpe.tex       # Evolución arquitectónica U-Net 1D y Optuna TPE
│   ├── 03_resultados_etapas.tex      # Métricas y validación cruzada
│   ├── 04_conclusiones_futuro.tex    # Conclusiones preliminares
│   ├── 04_resultados_etapas.tex      # Resultados en 5 etapas y análisis SOTA
│   ├── 05_conclusiones_futuro.tex    # Cumplimiento de objetivos y trabajo futuro
│   ├── 05_referencias.tex            # Diapositivas de transición de referencias
│   ├── 06_referencias.tex            # Referencias bibliográficas completas
│   ├── 07_anexos.tex                 # Metodología y material complementario
│   └── 08_anexos_adicionales.tex     # Anexos técnicos adicionales
├── .gitignore             # Filtro de archivos auxiliares de LaTeX
├── LICENSE                # Licencia MIT
├── main.pdf               # Presentación compilada en formato PDF
├── main.tex               # Archivo raíz de la presentación (Beamer)
├── README.md              # Documentación del repositorio
└── references.bib         # Archivo BibTeX con las fuentes citadas
```

---

## ⚙️ Requisitos y Compilación

### Requisitos previos
- Distribución de LaTeX instalada: [MiKTeX](https://miktex.org/) o [TeX Live](https://www.tug.org/texlive/).
- Motor de compilación: `pdflatex` (formato 16:9, compatible con `beamer`).

### Compilación por línea de comandos

Para compilar la presentación y generar `main.pdf`:

```bash
pdflatex -synctex=1 -interaction=nonstopmode main.tex
bibtex main
pdflatex -synctex=1 -interaction=nonstopmode main.tex
pdflatex -synctex=1 -interaction=nonstopmode main.tex
```

### Compilación en Visual Studio Code
El repositorio incluye la configuración de la extensión **LaTeX Workshop** en `.vscode/settings.json`. Basta con abrir `main.tex` y presionar:
- `Ctrl + Alt + B` (o guardar el archivo si el auto-build está habilitado).

---

## 📄 Licencia

Este proyecto está bajo la Licencia [MIT](LICENSE).
