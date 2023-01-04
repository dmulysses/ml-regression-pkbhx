# Machine Learning | Predicting Hydrogen-Bond Basicity



![python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![Sckit-Learn](https://img.shields.io/badge/Scikitlearn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)

# Problem Scope
  The inter- and intramolecular interactions are essential in physical, chemical, and biological properties. Within the various existing interactions, such as ionic strength and Van Der Waals interactions, hydrogen bonding (HB) strongly influences properties such as the solubility of inorganic and organic compounds, reactivity of molecules in the ground and excited states, activity of drugs, crystal packing, protein structures, and the catalytic activity of enzymes.
  
  
  The debate to define a hydrogen bond began in the first decades of the XX century and has evolved until we reached the current definition. In 2011, the International Union of Pure & Applied Chemistry (IUPAC) proposed the following recommendation:
> The hydrogen bond is an attractive interaction between a hydrogen atom from a molecule or a molecular fragment X–H in which X is more electronegative than H, and an atom or a group of atoms in the same or a different molecule, in which there is evidence of bond formation.

   We can represent the description given by IUPAC in the form of a chemical equation like the one shown below. In this case, the hydrogen bond (denoted as three dots) is formed by the interaction between a molecule containing the X–H moiety denominated as hydrogen bond donor (HBD), and the molecule that contains the atom that will interact with the X-H forming a bond, called as hydrogen bond acceptor (HBA).

$$HBA + HBD \rightleftharpoons HBA\cdots HBD$$

  From this chemical representation, we can write a mathematical equation using the concentration correlation to describe the strength of the interaction between HBD and HBA represented by the complexation constant K.

$$\mathit{K} = \frac{[HBA\cdots HBD]}{[HBA][HBD]}$$

or in the commonly used logarithmic form

$$p\mathit{K}_{BHX}= log\mathit{K} = log\frac{[HBA\cdots HBD]}{[HBA][HBD]}$$
