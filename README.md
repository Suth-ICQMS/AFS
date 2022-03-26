# Atomic Feature Set (AFS)  
The supporting materials of cuprate superconducting materials above liquid nitrogen temperature from machine learning  
- ① This software is written as a simple and practical exe program, which does not need other supporting environment, but can be used directly on the Windows system.  
- ② The software is used to extract the characteristics of simple chemical formula, temporarily **does not support** -- **"chemical formula with brackets, hydrate symbols, symbols such as electron valence"** if you have special needs can contact the author, contact information see the console.  
- ③ The limit of features dimension are 1000 (the results follows your feature file), 10000 is the most characters per line, you can not only use the feature file of the basic nature of element physics we provide but also customize it to add the features you want.  
- ④ elements characteristics of the basic characteristics of physical files to pay-per-tweet.  CSV, for example ("https://www.nature.com/articles/npjcompumats201628) in the CSV" we collected the elements of the basic physical quantities given in the pay-per-tweet, specific characteristics of the original magpe), please strictly follow pay-per-tweet.  CSV file input format, and corrected before populate CSV file name is: Fillfeature.  CSV.  
- ⑤ Ensure fillfeature.csv (feature file) and data.CSV (require only the column of chemical formula and no other redundant characters) in the same folder as EXE software.   
- ⑥ Run the software, input ICQMSicqms, get out.  CSV file, namely extraction of chemical formula characteristics.  
- ⑦ Copy the input case in example, copy EXe into the folder to run, and get the out.csv file.  
- ⑧ It is noted that when Fillfeature appears in data.CSV file.  CSV features cannot be extracted, we use the common method of 0 to fill, when abnormal data such as the denominator is 0, the feature is calculated as -1.   

| Feature | Specific Meaning |   
| :----:| :----: |  
| Number | The atomic number of the element |  
| MendeleevNumber | The mendeleev number of the element |  
| AtomicWeight | Mass of the atom |  
