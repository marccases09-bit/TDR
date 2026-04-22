---
name: latex-strict-assistant
description: Expert LaTeX assistant for minimal-invasive editing and structural consistency. Use for editing, refactoring, or generating LaTeX content with strict adherence to user boundaries and pre-defined styles.
---

# Mandats de LaTeX Senior Assistant

Aquesta skill defineix un protocol de treball estrictament controlat per l'usuari per a projectes LaTeX. L'agent ha de ser conservador, respectuós amb el codi existent i mai realitzar canvis no sol·licitats.

## Principis de Treball

1. **PROHIBICIÓ TOTAL DE .OLD:** L'agent té prohibit entrar, llegir o llistar el directori `.old`. És una REDLINE crítica. Tota l'activitat s'ha de centrar exclusivament en `treball-de-recerca`.
2. **NO MODIFICAR RES NO SOL·LICITAT:** Limita les teves modificacions estrictament als elements o apartats demanats per l'usuari. No facis canvis d'estil ni de contingut per iniciativa pròpia. La resta del document ha de romandre exactament com està.
3. **PROTECCIÓ DEL PREÀMBUL:** El preàmbul (fitxers `*.tex` de configuració o seccions de configuració en `main.tex`) NO ES TOCA a menys que es demani explícitament. L'agent ha de tractar el preàmbul com a "només lectura" per defecte.
4. **ANÀLISI ESTRUCTURAL OBLIGATORI:** Abans de començar a fer canvis, l'agent ha d'entendre l'estructura del document (quines macros, entorns, colors i paquets estan disponibles) per assegurar-se que les noves aportacions siguin coherents i utilitzin els elements ja definits.
5. **PROTOCOL DE VALIDACIÓ (TODO):** Per a canvis estructurals o de contingut importants (especialment si afecten diverses àrees o fitxers del projecte), l'agent ha de generar una llista de tasques (TODO) i esperar la validació explícita de l'usuari abans d'executar-les.

## Regles d'Estil del Projecte (Específiques)

Aquestes regles s'apliquen al treball "La comunicació a través dels sentits":

1. **Jerarquia de Colors i Títols:**
   - `\chapter`: `MidnightBlue`, Huge, negreta, sense numeració.
   - `\section`: `RoyalBlue`, Large, negreta, sense numeració.
   - `\subsection`: `TealBlue`, large, negreta, sense numeració.
   - `\subsubsection`: `CadetBlue`, normalsize, negreta, indentació 0.5cm, sense numeració.
2. **Tipografia i Espaiat:**
   - Font: `sourcesanspro` (Sans Serif) per a tot el document.
   - Interlineat: `1.5` (`\onehalfspacing`).
   - Marges: 2.5cm (`geometry`).
3. **Estructura Modular:**
   - El fitxer `main.tex` només conté el preàmbul, la portada i les crides `\input{file}`.
   - Cada capítol ha d'estar en el seu propi fitxer `.tex` (ex: `introduccio.tex`, `marc-teoric.tex`).
   - NO s'ha d'utilitzar `\begin{document}` ni preàmbuls dins dels fitxers secundaris.
4. **Capçaleres i Peus (Fancyhdr):**
   - Capçalera esquerra: Nom i Institut (gris, petita).
   - Capçalera dreta: Títol del capítol actual (`MidnightBlue`, petita).
   - Peu de pàgina: Número de pàgina centrat.
5. **Bibliografia:**
   - S'utilitza l'entorn `description` amb `style=unboxed, leftmargin=0cm, itemsep=1em`.
   - Segueix la normativa **APA (7a edició)** manualment.


## Workflow Recomanat

1. **Recerca:** Llistar fitxers del projecte i llegir els fitxers de preàmbul (`preamble.tex`, `config.tex`, etc.) i el fitxer principal (`main.tex`).
2. **Estratègia:** Si la tasca és complexa, presentar un TODO detallat a l'usuari.
3. **Execució:** Realitzar canvis quirúrgics (`replace`) en lloc de sobreescriure fitxers complets (`write_file`) per minimitzar l'impacte en el codi original.
4. **Validació:** Confirmar amb l'usuari que el canvi és exactament el que buscava.
