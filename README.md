# PHYS 25000 Final Project - Where's Waldo?

Public repository for final project - Data has been removed to observe copyright laws


To fulfill requirements for PHYS 25000, Computational Physics at the University of Chicago:

For source code see "main.py"

This project is a fun, simple machine learning approach to solving Where's Waldo books computationally.  Data was scanned in color from every Waldo book I could find at the local library (not included here for obvious reasons).  The dataset was randomly split into training, validation, and testing sets, and a U-Net architecture was used to semantically segment Waldo from his surroundings.  All truth files were hand drawn as masks of Waldo's head.  The dataset was augmented during training with a random jitter region of interest (ROI), which simultaneously increased the available images to train on and ensured that smaller crops were taken of the appropriate size without losing resolution.  The testing was done with a scanning ROI and pieced together, with Waldo's location being determined by the largest deteced binary object from the network.  Waldo was correctly identified in 9/12 images, Wenda in 2/11 (a near miss), and missed once (a red and white striped dino...)
