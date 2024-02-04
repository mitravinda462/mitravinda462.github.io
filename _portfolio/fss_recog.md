---
title: "Face Sketch-Photo Synthesis & Recognition"
excerpt: "Framework to synthesize face sketches from photos and vice-versa along with facial recognition"
date: Jan - Dec 2021
collection: portfolio
---

I worked under Prof. Mamatha HR in devising a framework that can help mitigate the challenge faced by
the law enforcement in accurately identifying faces of criminals through forensic sketches or mugshot
photos. My research led me to discern the need to build a framework which is inclusive of skin and hair
colors of the face-photos. I devised separate frameworks to convert face-sketches to face-photos and
vice-versa. 
1. Face-sketch synthesis framework
![Screenshot 2024-02-03 200328](https://github.com/mitravinda462/mitravinda462.github.io/assets/53876415/9e5a3c61-ea9c-48b3-9332-b2e32b99eb86)

I used image processing methodologies like 2 scale image decomposition and bilateral filtering to convert photos to sketches.
 
2. Face-photo synthesis framework
![Screenshot 2024-02-03 200456](https://github.com/mitravinda462/mitravinda462.github.io/assets/53876415/c459655c-3c05-41bd-a582-c8cebad14b83)

I used the face-sketch synthesis module to generate a face-sketch database of the existing face-photo database, ‘CelebA’. I trained a 9 layered Convolutional Neural Network model to convert sketches to photos. 

3. Face recognition
![Screenshot 2024-02-03 200533](https://github.com/mitravinda462/mitravinda462.github.io/assets/53876415/6cdf5e37-fea5-4b62-948c-300a6359cd8b)

I finally used Linear Discriminant Analysis to perform facial recognition on face-photos and face-sketches. 

The framework also took care of variations like different skin tones and hair colors, absence of hair, presence of beard, mustache or spectacles. In addition to the statistical evaluation metrics like Feature Similarity Index Measure, Structural Similarity Index Measure, Universal image Quality Index, I conducted an online survey to rate the similarity between the original and generated images, thus capturing the human visual similarity perception.

The project can be found [here](https://github.com/mitravinda462/Face-photo-sketch-synthesis-and-Recognition)
