# Machine Learning | Predicting Hydrogen-Bond Basicity

![python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![Sckit-Learn](https://img.shields.io/badge/Scikitlearn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)

# Problem Scope
  The inter- and intramolecular interactions are pivotal in physical, chemical, and biological properties. Within the various existing interactions, such as ionic strength and Van Der Waals interactions, hydrogen bonding (HB) strongly influences properties such as the solubility of inorganic and organic compounds, reactivity of molecules in the ground and excited states, activity of drugs, crystal packing, protein structures, and the catalytic activity of enzymes.
  
  
  The debate to define a hydrogen bond began in the first decades of the XX century and has evolved until we reached the current definition. In 2011, the International Union of Pure & Applied Chemistry (IUPAC) proposed the following recommendation:
> The hydrogen bond is an attractive interaction between a hydrogen atom from a molecule or a molecular fragment X–H in which X is more electronegative than H, and an atom or a group of atoms in the same or a different molecule, in which there is evidence of bond formation.

   We can represent the description given by IUPAC in the form of a chemical equation like the one shown below. In this case, the hydrogen bond (denoted as three dots) is formed by the interaction between a molecule containing the X–H moiety denominated as hydrogen bond donor (HBD), and the molecule that contains the atom that will interact with the X-H forming a bond, called as hydrogen bond acceptor (HBA)

$$HBA + HBD \rightleftharpoons HBA\cdots HBD$$

  From this chemical representation, we can write a mathematical equation using the concentration of the species to describe the strength of the interaction between HBD and HBA represented by the complexation constant _K_

$$\mathit{K} = \frac{[HBA\cdots HBD]}{[HBA][HBD]}$$

or in the commonly used logarithmic form

$$p\mathit{K}_{BHX}= log\mathit{K} = log\frac{[HBA\cdots HBD]}{[HBA][HBD]}$$

It is interesting to note that if we use a single HBD molecule as a reference, it becomes possible to construct a scale of hydrogen bonding strength for different HBA molecules, i.e., the value of the _K_ or the p*K*<sub>BHX</sub> becomes the measure of the ability of the HBA molecule to form a hydrogen bond. In 2009, Laurence and co-workers reported in [The Journal of Medicinal Chemistry](https://pubs.acs.org/doi/10.1021/jm801331y) a comprehensive database containing the experimental p*K*<sub>BHX</sub> value from about 1100 HBA, using 4-fluorphenol as an HBD reference.

An extensive discussion including the historical review, basic principles, and experimental and theoretical determination of hydrogen bond is available in the excellent _Nature of the Hydrogen Bond: Outline of a Comprehensive Hydrogen Bond Theory_.

<a href="https://academic.oup.com/book/11749"/><img src="https://user-images.githubusercontent.com/8021054/210620687-ffb8cb2b-1bd3-4f3f-9a5e-c1f46c64e57b.PNG" height="400"/>

# Metric

The following metrics were used for evaluating the model performance.

Coefficient of determination ( $R^{2}$ ):

$$R^{2} = 1 - \frac{\sum_{i=1}^{n}(y_{i}-\hat{y_{i}})^{2}}{\sum_{i=1}^{n}(y_{i}-\bar{y}_{i})^{2}}$$

Root Mean Squared Error

$$RMSE(y, \hat{y}) = \sqrt{\frac{1}{n}\sum_{i=1}^{n}(y_{i}-\hat{y}_{i})^{2}}$$

Mean Absolute Error (MAE):

$$MAE = \frac{ \sum_{i=1}^{n}|y_{i}-\hat{y}_{i}|}{n}$$
