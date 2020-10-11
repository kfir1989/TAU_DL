# TAU_DL
Acoustic scene classification using convolutional denoising auto encoder



Abstract 

In this project,  we demonstrate how we applied convolutional neural networks for acoustic scene classification (ASC). We present the use of a convolutional denoising auto encoder (CDAE) to capture discriminative information underlying the audio, among other preprocessing methods such as Mel Spectrograms and Harmonic Percussive source separation (HPSS). The experimental results show that the proposed network structure along with the preprocessing methods effectively learn acoustic characteristics from the audio recordings, and their ensemble model significantly reduces the error rate further, exhibiting an accuracy of 0.842 on the evaluation set.



Appendix

https://github.com/pranjaldatta/Denoising-Autoencoder-in-Pytorch
https://www.kaggle.com/talmanr/cnn-with-pytorch-using-mel-features




Results

ALGORITHMS	VALIDATION ACC.	EVALUATION ACC
MONO (MEL)	0.946	0.795
HPSS	0.872	0.675
ENCODED	0.956	0.812
ENSEMBLE	0.964	0.842


Future Work

We would like to suggest several possible improvements as future work. The first is to test the impact of different noise types (spectrogram corruption) on final classification performance. As an alternative, we would suggest to consider using a contractive auto encoder instead of denoising auto encoder, thus force the model to learn how to contract a group of inputs into a smaller group of outputs. Second is using different margin parameters for HPSS decomposition to exploit the full advantage out of it.



