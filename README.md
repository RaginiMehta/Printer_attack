# Paper To be Implemented : Texture Based Attacks on Intrinsic Signature Based Printer Identification

### Link to paper(need to signed in with school) : https://drive.google.com/drive/folders/1dCZdPDzNXtPb83_TDM2T2Khl4fVmR8cC

## Abstract : 
Several methods exist for printer identification from a printed document. We have developed a system that performs printer identification using intrinsic signatures of the printers. Because an intrinsic signature is tied directly to the electromechanical properties of the printer, it is difficult to forge or remove. There are many instances where existance of the intrinsic signature in the printed document is undesireable. In this work we explore texture based attacks on intrinsic printer identification from text documents. An updated intrinsic printer identification system is presented that merges both texture and banding features. It is shown that this system is scable and robust against several types of attacks that one may use in an attempt to obscure the intrinsic
signature.

### Keywords: document security, secure printing, printer identification, banding

## Ongoing Report : 

https://docs.google.com/document/d/1cTGTo6ci8M2kGMI3o8cecRoUmg6FhsRfl0oEGGIPEt0/edit?usp=sharing

## Steps : 

1. Get PDFs -> Images
2. Get individal Charecters -> 'e'  
3. Extract Features :
	a. Variance/Entropy
	b. GLCM features
	c. DFT Features
4. Classifier -> Majority Vote -> Output Class
5. Design attacked versions of the test image
6. Try Classifying

### Project Directory Structure

The directory structure for this project is as follows:

. ├── Attacks.ipynb ├── Dataset_OG │ ├── banded_image_10_0.01.jpg │ ├── banded_image_10_0.04.jpg │ ├── banded_image_10_0.1.jpg │ ├── banded_image_5_0.1.jpg │ └── BASE_OG.jpg ├── dist_csvs │ ├── class_label.csv │ ├── 10_X_column_i.csv ├── feature_extr.ipynb ├── feature_plot.ipynb ├── file_structure.txt ├── indiv_scripts │ ├── DFT.ipynb │ ├── get_e.ipynb │ └── GLCM.ipynb ├── plots │ ├── dft_lda_plot.png │ └── lda_grid_plot.png ├── Printer_Mimic.ipynb ├── README.md ├── Ref_PDFs │ ├── GLCM.pdf │ └── Texture_based_attacks_on_intrinsic_signature_based_printer_identification.pdf ├── saved_e │ └── 5_printers │ ├── 50_extracted_e's │ └── ef_50.pkl_files ├── SVM_trainedModels │ ├── svm_col10.joblib │ ├── svm_col1.joblib │ ├── svm_col2.joblib │ ├── svm_col3.joblib │ ├── svm_col4.joblib │ ├── svm_col5.joblib │ ├── svm_col6.joblib │ ├── svm_col7.joblib │ ├── svm_col8.joblib │ └── svm_col9.joblib ├── test_images │ ├── marked_es.png │ ├── output_with_boxes.png │ ├── test_0.png │ ├── test_1.jpeg │ ├── test_2.png │ ├── test_3.png │ ├── test4.jpg │ ├── test5.png │ └── test_6.jpg ├── Testing_Dataset │ ├── banded_image_10_0.01_7 │ ├── banded_image_10_0.04_7 │ ├── banded_image_10_0.1_7 │ ├── banded_image_5_0.1_7 │ └── BASE_OG_7 ├── Testing_images │ ├── attack_fixed_freq_binarized.jpg │ ├── attack_fixed_freq.jpg │ ├── attack_freq_hopping_binarized.jpg │ ├── attack_freq_hopping.jpg │ ├── attack_gaussian_noise.jpg │ └── TESTING_CV.jpg ├── train_features.ipynb └── Training.ipynb
26 directories, 344 files
