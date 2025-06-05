# Generating Antibacterial Molecules using Deep Learning
## Project Description

The goal of this project is to apply Deep Learning techniques to generate novel candidate molecules with potential antibacterial activity. We aim to develop a generative model that learns from known antibacterial molecules and creates new molecular structures that could act as antibiotics.
We will use the ChEMBL database, focusing on molecules tested against bacteria focusing on Escherichia coli. For each molecule, we retrieve:

  * Its structure in SMILES format (like a string).
    
We train a Variational Autoencoder (VAE) to learn a latent representation of the molecules. The model is used to generate new SMILES strings (new molecular structures)

We  train a simple classifier to predict whether the generated molecules might have antibacterial activity. We also apply chemical filters (Lipinski's Rule of Five, QED score, provided in the dataset) to ensure chemical viability.

