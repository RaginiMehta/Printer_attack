# Paper To be Implemented : 
Texture Based Attacks on Intrinsic Signature Based Printer Identification

### Link to paper(need to signed in with school) : https://drive.google.com/drive/folders/1dCZdPDzNXtPb83_TDM2T2Khl4fVmR8cC

## Abstract : 
Several methods exist for printer identification from a printed document. We have developed a system that performs printer identification using intrinsic signatures of the printers. Because an intrinsic signature is tied directly to the electromechanical properties of the printer, it is difficult to forge or remove. There are many instances where existance of the intrinsic signature in the printed document is undesireable. In this work we explore texture based attacks on intrinsic printer identification from text documents. An updated intrinsic printer identification system is presented that merges both texture and banding features. It is shown that this system is scable and robust against several types of attacks that one may use in an attempt to obscure the intrinsic
signature.

### Keywords: document security, secure printing, printer identification, banding

## Ongoing Report : 

https://docs.google.com/document/d/1NaS4cRLZlODuyYB9pB7OZBjWaRNupM2Noc6ykY5M2KU/edit?tab=t.0

## Steps : 

1. Get PDFs -> Images
2. Get individal Charecters -> 'e'  - Done
3. Extract Features 
	a. Variance/Entropy
	b. GLCM features
	c. DFT Features
4. Classifier -> Majority Vote -> Output Class
5. Design attacked versions of the test image
6. Try Classifying
