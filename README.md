Repositorio de Publicaciones: Sismicidad Lunar y Generación de Acelerogramas Sintéticos

Este repositorio contiene únicamente las publicaciones derivadas de los proyectos  No incluye código fuente, datos ni software; solo documentos académicos.

Publicaciones
1. Tesis de Pregrado

Título: Generación de Acelerogramas Sintéticos para la Luna Basados en la Metodología de Kanai-Tajimi
Autor: Oscar Alejandro Arcila Giraldo
Co-directores: Daniel Gómez Pizano, PhD; Alejandro Cruz Escobar, MSc
Institución: Universidad del Valle, Facultad de Ingeniería, Escuela de Ingeniería Civil y Geomática
Año: 2025
Archivo: UnderGraduateDssertationOscarArcila.pdf

Resumen:
La idea de colonizar la Luna para aprovechar todas sus ventajas geográficas, económicas y tecnológicas plantea la necesidad de construir hábitats permanentes. La construcción de estas estructuras debe considerar la amenaza sísmica. No obstante, la poca disponibilidad de registros con características adecuadas requiere el uso de metodologías alternativas que permitan generar registros nuevos a partir de los existentes. Este trabajo calcula la deconvolución regularizada de los registros tipo superficial del proyecto Apollo, registrados con sismómetros tipo LP de disposición horizontal, posteriormente emplea un algoritmo derivado de la metodología de Kanai–Tajimi y la optimización de enjambres para caracterizar los registros. Se obtuvieron los sismogramas calibrados de los registros, se caracterizaron estos en el dominio del tiempo y frecuencia y se construyó una aplicación para automatizar y simplificar el proceso. Adicionalmente, se desarrolló una metodología que permite la deconvolución de los registros LP del proyecto Apollo de componente horizontal, caracterizando de manera satisfactoria estos registros e implementando un software para la aplicación fácil y rápida de estos resultados en la generación de sismogramas sintéticos para la Luna. La metodología desarrollada puede adaptarse con relativa facilidad a otros tipos de eventos, como por ejemplo los producidos por impacto de meteoroide o a registros clasificados como profundos. Finalmente, los resultados se encuentran limitados principalmente debido al número de registros disponibles, lo que demuestra la necesidad de nuevos estudios sísmicos en la Luna.

Palabras clave: moonquake, proyecto Apollo, deconvolución, sismos sintéticos.
2. Artículo de Conferencia

Título: Preliminary approach to assess the seismic hazard on the Moon
Autores: Paula Cadena, Santiago Ruiz, Oscar Arcila, Vanessa Prado, Andrés Patiño, Daniel Gómez, Alejandro Cruz, Lina Ospina, Isabel Gómez
Publicación: 2020 Congreso Internacional de Innovación y Tendencias en Ingeniería (CONIITI)
Año: 2020
Páginas: 1–6
DOI: 10.1109/CONIITI51147.2020.9240257
Archivos:

    Cadena et al. - 2020 - Preliminary approach to assess the seismic hazard on the Moon.pdf

    Preliminary approach to assess the seismic hazard on the Moon.bib

Abstract:
The interest and desire of humanity to build extraterrestrial habitats brings with it great scientific and engineering challenges. To guarantee the safety and resilience of these habitats, it is necessary to characterize the hazards to which they will be exposed. Based on seismic information collected by The Apollo space program between 1969 and 1977 was developed a database tool with the purpose of allowing any researcher to manipulate and process the seismic signals of the Moonquakes. On the other hand, this paper presents an overview to assess the seismic hazard at a specific site on the Moon, using a probabilistic seismic hazard model (PSHA). To perform this analysis, only shallow Moonquakes are considered, since these are the biggest in magnitude and most energetic type of Moonquake recorded. Taking into account there have been registered only 28 shallow Moonquakes, which do not provide complete information, a Kanai-Tajimi filter is used to generate probable artificial accelerograms that adjust to the observed events.

Index Terms: Resilient habitats, seismic hazard, Kanai-Tajimi filter, synthetic accelerograms.
Cómo Citar
Tesis
bibtex

@phdthesis{arcila2025moonquake,
  title={Generación de Acelerogramas Sintéticos para la Luna Basados en la Metodología de Kanai-Tajimi},
  author={Arcila Giraldo, Oscar Alejandro},
  year={2025},
  school={Universidad del Valle},
  address={Santiago de Cali, Colombia}
}

Artículo de Conferencia
bibtex

@INPROCEEDINGS{9240257,
  author={CADENA, PAULA and RUIZ, SANTIAGO and ARCILA, OSCAR and PRADO, VANESSA and PATIÑO, ANDRES and GÓMEZ, DANIEL and CRUZ, ALEJANDRO and OSPINA, LINA and GÓMEZ, ISABEL},
  booktitle={2020 Congreso Internacional de Innovación y Tendencias en Ingeniería (CONIITI)},
  title={Preliminary approach to assess the seismic hazard on the Moon},
  year={2020},
  pages={1-6},
  doi={10.1109/CONIITI51147.2020.9240257}
}

Agradecimientos

Este trabajo recibió financiamiento del proyecto de convocatoria interna de la Universidad del Valle titulado "Metodología para la caracterización de la amenaza sísmica, generación de sismos sintéticos y espectros de diseño para la Luna" (21078).

Agradecemos a ISAS/JAXA por su servicio gratuito de base de datos DARTS, el cual proporcionó los registros sísmicos del proyecto Apollo.

    This research made use of data obtained from Data ARchives and Transmission System (DARTS), provided by Center for Science-satellite Operation and Data Archive (C-SODA) at ISAS/JAXA.

Licencia

Los documentos aquí depositados se comparten con fines académicos y de investigación. Para cualquier otro uso, por favor contactar a los autores.
Contacto

Oscar Alejandro Arcila Giraldo
Escuela de Ingeniería Civil y Geomática
Universidad del Valle
Santiago de Cali, Colombia
Email: oscar.arcila@correounivalle.edu.co

# Synthetic Moonquake Generator (SMG)

![SMG Logo](Images/icon48.jpg)

**Version:** 1.0  
**Authors:** Oscar Arcila, Daniel Gómez, Alejandro Cruz  
**Institution:** School of Civil Engineering, Universidad del Valle, Colombia  
**License:** Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)

---

## Description

**Synthetic Moonquake Generator (SMG)** is a MATLAB application designed to generate synthetic lunar earthquakes (*moonquakes*), specifically adapted to reproduce surface-type lunar seismic records from long-period, horizontally oriented sensors of the Apollo seismic network.

The application employs a modified **Kanai–Tajimi methodology** for the generation of synthetic moonquake ground motions.

SMG allows users to:

- Generate synthetic moonquake accelerograms.
- Define white-noise characteristics.
- Design and apply band-pass filters.
- Define temporal envelopes.
- Scale synthetic records to a desired Peak Ground Acceleration (PGA).
- Calculate seismic response spectra.
- Visualize generated signals and spectra.
- Export numerical results as text files.
- Export figures in MATLAB `.fig` format.
- Save and load projects using `.smg` files.

The application was developed using **MATLAB R2022a** and compiled as a standalone executable using **MATLAB Compiler**.

---

## Features

### Main Application

- Graphical user interface.
- Main window with menu bar.
- Two main tabs:
  - **Synthetic Accelerogram**
  - **Response Spectrum**
- Project management through `.smg` files.

### File Menu

- Open
- Save As
- Close

### Help Menu

- User Manual
- File Association
- License Agreement
- About

---

## Synthetic Accelerogram

The **Synthetic Accelerogram** tab allows the user to generate a synthetic moonquake accelerogram through a stochastic simulation workflow.

### White Noise

Defines:

- Event duration.
- Sampling frequency.

### Band-Pass Filter

Provides two configuration modes:

#### Observed Values

Uses predefined filtering parameters based on observed lunar seismic records.

The filter includes:

- High-pass cutoff frequency.
- Low-pass cutoff frequency.
- Damping ratios.
- Filter parameters.

#### User Values

Allows the user to define:

- High-pass cutoff frequency.
- Low-pass cutoff frequency.
- Damping ratios.
- Filter order.

The user-defined filter is based on a Butterworth filter with variable order.

### Temporal Envelope

Defines the temporal evolution of the synthetic moonquake.

The envelope is controlled through parameters including:

- `t1`
- `a`
- `t2`
- `c`

Predefined observed values are available for different moment-magnitude ranges:

- `Mw = 2.7–3.2`
- `Mw = 3.3–3.6`
- `Mw = 3.7–4.1`

User-defined parameters can also be entered manually.

### PGA

The PGA panel allows the synthetic record to be scaled to a desired **Peak Ground Acceleration**.

### Plot Panel

The application provides six plots:

1. White-noise accelerogram.
2. White-noise Power Spectral Density (PSD).
3. Filter Bode amplitude.
4. Filter Bode phase.
5. Synthetic moonquake accelerogram with temporal envelope and RMS.
6. Synthetic moonquake PSD.

### Export

The application provides:

- **Export Figures** — exports figures as MATLAB `.fig` files.
- **Export Accelerogram** — exports the synthetic accelerogram as a text file.

---

## Response Spectrum

The **Response Spectrum** tab calculates the seismic response spectra of the generated synthetic moonquake.

### Damping Ratio

Defines the damping ratio used in the response-spectrum calculation.

### Response Spectrum Periods

Defines:

- Minimum period (`Tmin`).
- Maximum period (`Tmax`).
- Number of periods (`Tnum`).

### Gravitational Acceleration

Defines the gravitational acceleration magnitude used for the calculations.

### SpecMQ

The `SpecMQ` function calculates the seismic response spectra of the synthetic moonquake.

### Plot Panel

The response-spectrum tab provides five plots:

1. Displacement.
2. Velocity.
3. Acceleration.
4. Pseudo-velocity.
5. Pseudo-acceleration.

### Export

The application provides:

- **Export Figures** — exports response-spectrum figures as MATLAB `.fig` files.
- **Export Spectra** — exports numerical response spectra as text files.

---

## Exported Results

### Synthetic Accelerogram

The synthetic accelerogram is exported as a text file.

The exported data contains:

| Column | Description |
|---|---|
| 1 | Time |
| 2 | Synthetic moonquake acceleration |

The file also contains descriptive information about the generated record.

### Response Spectra

The response spectra are exported as a text file containing the calculated spectral quantities.

The exported file includes the parameters used in the response-spectrum calculation.

---

## Project Files

SMG supports project files with the `.smg` extension.

A project file stores the values associated with a synthetic moonquake generation project and allows the project configuration to be restored later.

---

## File Association

To associate `.smg` project files with SMG:

1. Create an `.smg` file using **Save As** from the **File** menu.
2. Right-click the `.smg` file.
3. Select **Open with**.
4. Select **Choose an app on your PC**.
5. Navigate to the SMG installation directory:

```text
C:\Program Files\UniValle\SMG\application\
````

6. Select:

```text
SMG.exe
```

7. Click **Open**.
8. Select the SMG application icon.
9. Select **Always**.

After the association is configured, double-clicking an `.smg` file will open SMG and load the project values.

For detailed instructions, see:

```text
Docs/SMGFileAssociation.pdf
```

---

## Requirements

### Hardware

* 64-bit processor.
* 8 GB RAM or more.
* 5 GB of available disk space or more.

### Software

* Windows 10 or later.
* PDF file reader.
* MATLAB Runtime.

> **MATLAB is not required to run the compiled application.** MATLAB Runtime is installed with the application.

---

## Installation

1. Locate `SMG.exe`.
2. Right-click the installer and select **Run as administrator**.
3. Click **Next** in the installation wizard.
4. Select **Add a shortcut to the desktop** and click **Next**.
5. Proceed with the required MATLAB Runtime installation.
6. Accept the MATLAB Runtime license agreement.
7. Click **Install**.
8. Click **Finish** when the installation is complete.

The default installation directory is:

```text
C:\Program Files\UniValle\SMG\
```

---

## Building from Source

SMG was developed in **MATLAB R2022a** and compiled using **MATLAB Compiler**.

### MATLAB Runtime Download Information

The MATLAB Runtime download URL can be obtained from MATLAB by executing:

```matlab
com.mathworks.toolbox.compiler.MatlabRuntimeUtils.getMCRInstallerDownloadURL()
```

### Compilation Procedure

1. Open the project in MATLAB R2022a.

2. Configure the required MATLAB paths.

3. Comment out the following line in `SMG.m` when preparing the application for compilation:

```matlab
addpath(genpath(pwd));
```

4. Execute the required path configuration in the MATLAB interpreter:

```matlab
addpath(genpath(pwd));
```

5. Open **MATLAB Compiler** from the MATLAB **Apps** tab.

6. Configure the application.

7. Set the main file to:

```text
SMG.m
```

8. Configure the application information.

| Setting                     | Value                                      |
| --------------------------- | ------------------------------------------ |
| Main File                   | `SMG.m`                                    |
| Application Name            | `SMG`                                      |
| Version                     | `1.0`                                      |
| Author                      | Oscar Arcila, Daniel Gómez, Alejandro Cruz |
| Company                     | Universidad del Valle                      |
| Summary                     | Synthetic Moonquake Generator              |
| Default Installation Folder | `\UniVal\SMG\`                             |

9. Select the application icons and splash screen from the `Images` directory.

10. Add the code repository folder to:

**Files required for your application to run**

11. Add all required files from the `endUser` directory to:

**Files installed for your end user**

12. Click **Package** to generate the application installer.

---

## Repository Structure

```text
SMG/
├── Code/
│   ├── 01Main/
│   ├── 02GP/
│   ├── 03FP/
│   ├── 04TP/
│   ├── 05PGA/
│   ├── 06PlotAcc/
│   ├── 07ExportAccFig/
│   ├── 08ExportAcc/
│   ├── 09ZZ/
│   ├── 10TN/
│   ├── 11GG/
│   ├── 12SP/
│   ├── 13PlotSpec/
│   ├── 14ExportSpecFig/
│   └── 15ExportSpec/
│
├── Docs/
│   ├── SMGFileAssociation.pdf
│   ├── SMGLicenseAgreement.pdf
│   └── SMGUserManual.pdf
│
├── Images/
│   ├── icon48.jpg
│   ├── miniature.jpg
│   └── temporalWindow.jpg
│
└── SMG.m
```

---

## Documentation

Additional documentation is included in the `Docs` directory:

| Document                  | Description                          |
| ------------------------- | ------------------------------------ |
| `SMGUserManual.pdf`       | SMG user manual                      |
| `SMGFileAssociation.pdf`  | `.smg` file association instructions |
| `SMGLicenseAgreement.pdf` | Software license agreement           |

---

## Credits and Attribution

This project contains unmodified code from the original work:

**Image Mouse Zoom and Pan**

by **Dany Cabrera**.

The original work was published through the MATLAB File Exchange and distributed under a **Creative Commons Attribution-ShareAlike 3.0 Unported (CC BY-SA 3.0)** license.

Original project:

[https://la.mathworks.com/matlabcentral/fileexchange/67583-image-mouse-zoom-and-pan](https://la.mathworks.com/matlabcentral/fileexchange/67583-image-mouse-zoom-and-pan)

The attribution and licensing requirements applicable to the incorporated work must be preserved.

---

## License

This work is licensed under the:

**Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**

license.

For more information about the license:

[https://creativecommons.org/licenses/by-sa/4.0/](https://creativecommons.org/licenses/by-sa/4.0/)

---

## Authors

* **Oscar Arcila** — [oscar.arcila@correounivalle.edu.co](mailto:oscar.arcila@correounivalle.edu.co)
* **Daniel Gómez** — [daniel.gomez@correounivalle.edu.co](mailto:daniel.gomez@correounivalle.edu.co)
* **Alejandro Cruz** — [alejandro.cruz@correounivalle.edu.co](mailto:alejandro.cruz@correounivalle.edu.co)

**School of Civil Engineering**
**Universidad del Valle**
Colombia

---

## References

* Chopra, A. (2012). *Dynamics of Structures: Theory and Applications to Earthquake Engineering* (4th ed.). Prentice Hall.

* Clough, R., & Penzien, J. (2003). *Dynamics of Structures* (Third ed.). Computers & Structures, Inc.

---

## Version

**Synthetic Moonquake Generator — Version 1.0**

