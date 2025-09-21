# Writing the Manuscript

Jump to:

- [Creating publication-ready figures](#creating-publication-ready-figures)
- [Data and Code stored with appropriate links](#data-and-code-stored-with-appropriate-links)
- [Picking a Journal](#picking-a-journal)
- [Format Paper based on Author Guidelines](#format-paper-based-on-author-guidelines)

---

## How to build a story board for your journal article
[This template](https://docs.google.com/presentation/d/1mOs9GQeXzpdUz7oXsork9p4GuLu6hA_ecqcAbT4xpFY/edit?slide=id.p#slide=id.p) should be used when you are at the beginning of writing your manuscript. This will help guide you on the content of your paper and finalizing your figures. 

When using this template, go to `File > Make a copy` to use and save it to your own drive.  

---

## Creating publication-ready figures
Creating figures takes multiple iterations. Here are some general guidelines for intuitive, understandable, and accurate publication-ready figures. 

![anatomy of figure](../images/anatomy_of_figure.png)

### Use of Color 
- Match color scale type to data (sequential, diverging, categorical) 
![color scale](../images/color_scale.png)
- Be consistent with color choices across the paper 
- Ensure accessibility (colorblind-friendly, high contrast) 
![color blindness](../images/color_blindness.png)

### Symbology
- Differentiate variables with one visual cue (color, line type, symbol). If color is used to differentiate, oftentimes a different line type of symbol than the standard is not necessary. For example, it is unnecessary to have symbols and colors for the same thing. 
![symbology](../images/symbology.png)
- Keep symbology consistent across all figures. 
- Make sure symbols and line types are readable at publication size. 
- Always simplify - avoid unnecessary symbol variations. 

### Layout & Text
- Scale figures to fit the page/half-page without excess white space 
- Maintain consistent subplot spacing and alignment 
- Label all axes (with units) and provide clear legends 
- Avoid repeating identical legends across subplots 
- Add subplot lettering (a, b, c, …) where needed
- Keep text legible - no font smaller than size 9
- Remove unnecessary borders on legends 
- Use annotations to guide interpretation

### Maps 
- Include scale bar and north arrow
- Add inset maps when the location context is unclear 
- Preserve the correct aspect ratio to avoid stretched maps 
- Use consistent basemaps and features across multiple maps 
- Ensure basemap/reference info supports the data without distracting from it

### Accessibility 
- Provide alt text for all figures
- Check and maintain sufficient color contrast 
- Test figures with a [colorblind simulator](https://www.color-blindness.com/coblis-color-blindness-simulator/)
- Use more than color alone to convey meaning 
- Provide data tables alongside graphics when possible

---

## Data and Code stored with appropriate links
We are dedicated to open science and reproducibility of our work. Having data and codes properly stored to make this possible is essential. Data is often stored in the GitHub repository itself, but if files are too large (>100 MiB), it is necessary to store them on online databases like Zenodo or CyVerse. Codes should be stored in the GitHub repository for your manuscript. 

It is important to note that the data being stored is only data that you have processed or analyzed. **DO NOT** upload raw data from the source. Instead, include instructions on how to download the data from the source in a Jupyter notebook.

In general, these are the contents that your GitHub repository should contain: 

- /code/ : folder containing all your codes and/or notebooks
- /data/ : folder containing the data needed 
- /results/ : folder containing all the figures in your paper and code/notebook that creates all these figures
- environment.yml or requirements.txt : file to re-create the virtual environment 
- README.md : main readme file that will contain instructions on cloning the repository and its content overview. Very important to have citation information included at the very top. 

These are some examples you can follow: 

- [https://github.com/condon-lab/De-la-Fuente_2024_Hydro-LSTM](https://github.com/condon-lab/De-la-Fuente_2024_Hydro-LSTM)
- [https://github.com/condon-lab/Tadych_2024_AZGroundwaterWells](https://github.com/condon-lab/Tadych_2024_AZGroundwaterWells)

Example of external storage for data: 

- Condon, L. (2024). Datasets supporting a Deep-Learning Based Parameter Inversion Framework for Large-Scale Groundwater Models [Data set]. Zenodo. [https://doi.org/10.5281/zenodo.14517560](https://doi.org/10.5281/zenodo.14517560)

---

## Picking a Journal 
When picking out a journal, you want to first look at the journals you’ve most frequently cited in your introduction of your manuscript. This will give you a good starting point. Ask your advisor or co-authors for potential recommendations. 

Create a list of 4-6 potential journals and include the following information for your next meeting with Laura: 

1. Name of Journal & Scope
2. Impact Factor & Cite Score
3. Cost to Publish 

---

## Format Paper based on Author Guidelines
Check the journal’s author guidelines. Some journals provide templates to follow for submission, or some journals are format-free, meaning you can submit your manuscript as is with inclusion of things such as title, authors, affiliations, acknowledgements, competing interests, code and data availability, etc. 

Common things to consider when formatting: 

- Word count 
- Figure format
- Figure captions
- Table formats 
- Numbering sections (1, 2, 3, … 1.1, 1.2, 2.1, 2,2…, etc) 
- Double spacing and numbered lines

It is essential to follow these guidelines to ensure a smooth process and expedite your submission to the editor’s desk for review. 
