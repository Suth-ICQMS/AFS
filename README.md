# Atomic Feature Set (AFS)  
The supporting materials of cuprate superconducting materials above liquid nitrogen temperature from machine learning  
- ① This software is written as a simple and practical program, which does not need other supporting environment, but can be used directly on the Windows system.  
- ② The software is used to extract the characteristics of simple chemical formula, temporarily **does not support** -- **"chemical formula with brackets, hydrate symbols, symbols such as electron valence"** 
- ③ The limit of features dimension are 1000 (the results follows your feature file), 10000 is the most characters per line, you can not only use the feature file (see elemFeature) of the basic nature of element physics we provide but also customize it to add the features you want.  
- ④ Name the chemical formula file and feature file as data.csv and Fillfeature.csv respectively. Make sure your files are encoded in **UTF-8**, otherwise the first line may be garbled.  
- ⑤ Ensure Fillfeature.csv (feature file) and data.csv (require only the column of chemical formula and no other redundant characters,see example) in the same folder as AFS.exe.   
- ⑥ Double click AFS.exe, and select the mode for extracting features **input: ICQMSicqms**, so get the out.csv file.  

**Abbreviations vs. Physical Property Characteristics**
| Feature | Specific Meaning |   
| :----:| :----: |  
| Number | The atomic number of the element |  
| MendeleevNumber | The mendeleev number of the element |  
| AtomicWeight | Mass of the atom |  
| MeltingT  | Melting point of the elemental crystal | 
| Column | The number of columns in the periodic table | 
| Row | The number of rows in the periodic table | 
| CovalentRadius | Covalent bond radius of atoms | 
| Electronegativity | Electronegativity  of the atom | 
| Ns, Np, Nd, Nf, N Valence | s, p, d, f, total valence electron number of atoms | 
| Ns, Np, Nd, Nf, N Unfilled | s, p, d, f, total unfilled electron number of atoms | 
|PBE_PRACOR |  Partial core radius in VASP PBE-POTCAR file   | 
|PBE_RCORE | Outmost cutoff radius in VASP PBE-POTCAR file |  
|GSvolume_pa |  Volume of elemental monomers at atmospheric pressure in the ground state  |  
| GSmagmom  | Elemental singlet magnetism at ground state atmospheric pressure  |  
|SpaceGroupNumber | Number of the space group in which the elemental monomers are located  |  

**Symbolic vs. Operation of specific values**  

Vectors composed of physical properties under **cell processing**(Normalization by component proportions)
e.g. Max(Formula=Cu1Cr1O2,Feature=Number)--→The largest element in the periodic table is the 29th element of Cu, which has a specific gravity of 1/4 = 0.25 in the normalisation process of stoichiometric ratios.
| Symbolic | Operation |   
| :----:| :----: |  
| Max | Maximum value of cell processing feature | 
| Min | Minimum value of cell processing feature | 
| Mean | Arithmetic averaging of cell processing feature | 
| Range | Extreme differences of cell processing feature | 
| Reduce | Reduced-mass like peration of cell processing feature| 


 
 
The Supporting Information of **Cuprate superconducting materials above liquid nitrogen temperature from machine learning** .  

For the **model.summary()** of tensorflow including "=====", which makes .ipynb can not preview online. Plase download the .ipynb or browse .PDF online for detial.
