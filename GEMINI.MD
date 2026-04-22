# Context del Projecte de Recerca

Aquest fitxer conté el background necessari per entendre el treball que s'està realitzant. Les directrius tècniques de LaTeX han estat mogudes a una **skill** específica (`latex-research-workflow`).

## Informació General
- **Tema:** La competència entre espècies (Gecko lleopard vs. Isòpodes).
- **Institució:** Institut Escola de Sant Pol de Mar.
- **Objectius del Document LaTeX:** 
  - Assistència en el format del document.
  - Inserció de peus de pàgina.
  - Gestió de citacions d'imatges.
  - Manteniment de la bibliografia (Norma APA).
- **Normativa d'Estil:** 
  - Normes APA actuals.
  - Normativa específica de l'Institut Escola de Sant Pol de Mar.

## Directrius de Treball (Actualitzades)
- **Mínima Intervenció:** Respectar l'estructura modular actual (`\input{seccions/...}`).
- **Protecció del Preàmbul:** No modificar el fitxer `main.tex` (paquets, marges, colors) sense autorització expressa.
- **Rigor Científic:** Mantenir la distinció entre factors biòtics i abiòtics i la correcció taxonòmica.
- **Gestió de Cites:** Convertir els marcadors provisionals `[cite: XXX]` a referències APA reals vinculades a la bibliografia.

## Estat Actual del Projecte (Abril 2026)
- **Estructura:** Modular i neta (carpeta `seccions/`).
- **Seccions Inicials:** `introduccio.tex` i `objectius-hipotesis.tex` creades com a esborrany (pendents de redacció).
- **Marc Teòric:** Base conceptual sobre ecosistemes redactada. Seccions de biologia específica (animals) creades però buides.
- **Marc Pràctic:** Disseny experimental plantejat, però sense dades ni anàlisi de resultats.
- **Bibliografia:** Llista d'URLs sense format APA i sense vinculació directa amb el text.

## Llista de Tasques Pendents (To-Do List)

### 1. Completar Marc Teòric
- [ ] **Gecko lleopard:** Redactar subseccions de Dieta, Comportament, Dimorfisme, Reproducció, Especímens i Malalties.
- [ ] **Isòpode 1 (*Porcellio laevis*):** Redactar Taxonomia, Distribució, Característiques, Dieta, Comportament i Cicle de vida.
- [ ] **Isòpode 2 (*Armadillidium vulgare*):** Redactar Taxonomia, Distribució, Característiques, Dieta, Comportament i Cicle de vida.

### 2. Gestió Bibliogràfica i Cites
- [ ] Crear fitxer de referències (BibTeX o format APA manual).
- [ ] Substituir marcadors `[cite: XXX]` per cites APA reals al llarg de tot el document.
- [ ] Revisar i formatar la secció `bibliografia.tex` segons la normativa de l'institut.

### 3. Desenvolupament del Marc Pràctic
- [ ] Descriure detalladament el muntatge del terrari bioactiu (amb especificacions tècniques).
- [ ] Redactar el diari d'observacions (Resultats).
- [ ] Realitzar l'Anàlisi de Resultats comparant-los amb les hipòtesis inicials.

### 4. Format i Elements Visuals
- [ ] Inserir imatges i diagrames amb peus de pàgina i citació de la font.
- [ ] Revisió lingüística final (català) i coherència terminològica.
- [ ] Generar l'índex de figures i taules (si s'escau).
