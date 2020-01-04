We provided the best model (k-NN[3-NN]) as model file for kNN.model

How to use this model file:
1. Prepare your data frame using .csv format.
2. The columns in the first row should be coded as TexF463,TexF579,TexF592,TexF599,TexF618,'Tumor diameter',benign/malign.TexF463 represets wavelet-HL ngtdm Strength,TexF579 represents wavelet-LL glcm JointEnergy,TexF592 represets wavelet-LL glcm Imc2,TexF599 represents wavelet-LL firstorder Uniformity, TexF618 represents wavelet-LL glrlm GrayLevelNonUniformityNormalized, 'Tumor diameter' represents maximum 3D diameter of the lesion.
3. Please be careful about the lower and upper cases in coding. Otherwise, it will not work.
4. The last column, namely benign/malign, is the target in the classification tasks. It should be coded as Benign or Malign.
5. Please be careful about the feature scaling technique defined in the paper. Otherwise, it will not work.
6. An example for the data frame in .csv format should be like the following:
	TexF463,TexF579,TexF592,TexF599,TexF618,'Tumor diameter',benign/malign
	-0.294836,-0.680663,0.766632,-1.06809,-1.050198,-1.046394,Benign
	-0.520296,0.309119,0.676014,-0.133548,-0.061884,-1.222183,Malign
7. Simplest way for the external validation is to use WEKA explorer application.
