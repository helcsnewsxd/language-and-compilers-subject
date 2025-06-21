> [!note]
> This repository contains theoretical notes, practical exercises, and a final project developed for the Language and Compilers course of the Computer Science degree at FAMAF – Universidad Nacional de Córdoba.
>
> All materials are in Spanish, as they were written for academic use and submission.

# Lenguajes y Compiladores

El presente repositorio contiene todo el material correspondiente a la cursada de la materia de _Lenguajes y Compiladores_ de 5to año de la Licenciatura en Ciencias de la Computación de FAMAF durante el año 2025.

## Información general

Los temas que trata la materia se pueden ver en el [programa](./information/study_program.pdf) de la misma. Respecto al material, este está basado en el apunte de la materia y en el libro _Theories of Programming Languages_ de John C. Reynolds (1998).

El equipo docente está conformado por:

- Miguel Pagano
- Matilda Steinberg
- Martín Vilela Demetrio

## Contenido

### Teórico

<div align="center">

| Temas                                                  | Descripción                                                                                                                                                                     | Filminas                                                                                                                                                                           | Apunte                                                                                                                             |
| ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Introducción a la sintaxis y la semántica de lenguajes | Gramáticas abstractas <br /> Función semántica <br /> Variables y ligadura                                                                                                      | [(1)](./theory/slides/01-part_1-abstract_sintax_and_semantic.pdf) <br /> [(2)](./theory/slides/01-part_2-free_and_bound_variable_coincidence_and_substitution.pdf)                 | [PDF](./theory/notes/01-abstract_sintax.pdf)                                                                                       |
| El problema de dar significado a la recursión          | Órdenes parciales y dominios <br /> Morfismos y funciones continuas <br /> Teorema del menor punto fijo                                                                         | [(1)](./theory/slides/02-part_1-recursion_definition_posets_domains_predomains.pdf) <br /> [(2)](./theory/slides/02-part_2-continuous_functions_and_least_fixed_point_theorem.pdf) | [PDF](./theory/notes/02-meaning_of_recursion.pdf) <br /> [Ejemplo](./theory/notes/02-example_of_least_fixed_point_calculation.pdf) |
| Lenguaje imperativo simple                             | LIS <br /> Propiedades de la semántica: TC, TR, TS, LS                                                                                                                          | [(1)](./theory/slides/03-part_1-simple_imperative_language.pdf) <br /> [(2)](./theory/slides/03-part_2-simple_imperative_language.pdf)                                             | [PDF](./theory/notes/03-imperative_language.pdf)                                                                                   |
| LIS con fallas, semántica denotacional y operacional   | LIS con fallas <br /> Semántica operacional <br /> Teorema de Corrección                                                                                                        | [(1)](./theory/slides/04-part_1-lis_with_fails.pdf) <br /> [(2)](./theory/slides/04-part_2-operational_semantic.pdf)                                                               | [PDF](./theory/notes/03-imperative_language.pdf)                                                                                   |
| LIS con input y output                                 | Más sobre dominios <br /> Input y output                                                                                                                                        | [(1)](./theory/slides/05-list_with_input_and_output.pdf)                                                                                                                           | [PDF](./theory/notes/03-imperative_language.pdf)                                                                                   |
| Cálculo Lambda                                         | Sintaxis <br /> Reducción <br /> Evaluación <br /> Semántica Denotacional (normal, eager)                                                                                       | [(1)](./theory/slides/06-lambda_calculus.pdf)                                                                                                                                      | [PDF](./theory/notes/06-lambda_calculus.pdf)                                                                                       |
| Lenguajes Aplicativos                                  | Evaluación eager <br /> Evaluación normal <br /> Tuplas <br /> Semánticas denotacionales en profundidad <br /> Recursión                                                        | [(1)](./theory/slides/07-aplicative_languages.pdf)                                                                                                                                 | [PDF](./theory/notes/07-aplicative_languages.pdf)                                                                                  |
| Lenguajes Iswim-like                                   | (Des)Referencia <br /> Asignación <br /> Igualdad <br /> Fragmentos imperativos <br /> Estado y semántica operacional <br /> Fragmento aplicativo <br /> Semántica denotacional | [(1)](./theory/slides/08-iswim.pdf)                                                                                                                                                | [PDF](./theory/notes/08-iswim.pdf)                                                                                                 |

</div>

### Práctico

<div align="center">

| Guía | Enunciados                           | Soluciones                          |
| ---- | ------------------------------------ | ----------------------------------- |
| 1    | [PDF](./exercises/statements/01.pdf) | [PDF](./exercises/solutions/01.pdf) |
| 2    | [PDF](./exercises/statements/02.pdf) | [PDF](./exercises/solutions/02.pdf) |
| 3    | [PDF](./exercises/statements/03.pdf) | [PDF](./exercises/solutions/03.pdf) |
| 4    | [PDF](./exercises/statements/04.pdf) | [PDF](./exercises/solutions/04.pdf) |
| 5    | [PDF](./exercises/statements/05.pdf) | [PDF](./exercises/solutions/05.pdf) |
| 6    | [PDF](./exercises/statements/06.pdf) | [PDF](./exercises/solutions/06.pdf) |
| 7    | [PDF](./exercises/statements/07.pdf) | [PDF](./exercises/solutions/07.pdf) |
| 8    | [PDF](./exercises/statements/08.pdf) | [PDF](./exercises/solutions/08.tex) |
| 9    | [PDF](./exercises/statements/09.pdf) |                                     |
| 10   | [PDF](./exercises/statements/10.pdf) |                                     |
| 11   | [PDF](./exercises/statements/11.pdf) |                                     |

</div>

## Proyecto

El proyecto de la materia consistió en investigar y realizar un informe de un tema relacionado a esta (Lenguajes y Compiladores) a libre elección en base a nuestros gustos. En general, podía ser un tema específico del libro (un capítulo) o un tema libre. Nosotros elegimos _Decompilación_.

El informe, caso de uso y presentación se encuentran en este [repositorio](https://github.com/helcsnewsxd/decompilation-report) público donde se hace una vista general de la arquitectura de dcc, uno de los primeros decompiladores (hecho por Cifuentes y Gough), luego por las mejoras o nuevas ideas del esquema dinámico con BinRec y finalmente una presentación de herramientas de decompilación y análisis de binarios actuales junto con algunas aplicaciones y una demo en Ghidra.

## Laboratorio

El laboratorio de la materia consistió en realizar un intérprete del lenguaje que quieras en el lenguaje que prefieras. Podías hacerlo de forma libre o siguiendo los laboratorios de años pasados donde el intérprete era sobre LIS hecho en Haskell.

En mi caso, hice un intérprete (en C++) de una reducción de C/C++ con tipado dinámico (y otras variantes), basándome en el libro de [_Crafting Interpreters_](https://craftinginterpreters.com/). Agregué unit testing con Catch2 y documentación autogenerada con Doxygen. El repositorio puede encontrarse [aquí](https://github.com/helcsnewsxd/gsc-interpreter). Es probable que se sigan viendo cambios luego de la entrega del laboratorio (1era release) porque me gustó mucho para extenderlo como hobby.
