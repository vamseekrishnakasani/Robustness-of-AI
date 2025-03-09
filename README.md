## Robustness of AI: Defending Against Adversarial Attacks

This repository explores making AI models more robust against adversarial attacks, focusing on FGSM (Fast Gradient Sign Method) and different defense strategies.

###Key Features 
	•	FGSM Attack: Generates adversarial examples to test model weaknesses. \
	•	Adversarial Training: Improves CNN robustness by training with both clean and FGSM-attacked data. \
	•	VAE for Defense: Uses a Variational Autoencoder (VAE) to reconstruct and remove noise from FGSM images. \
	•	GAN for Detection: Uses a GAN’s discriminator to identify adversarial samples as anomalies.

###Results
	•	Baseline CNN (Clean Data): ~99% accuracy \
	•	CNN on FGSM Data: ~70-80% accuracy \
	•	CNN after Adversarial Training: ~95-98% accuracy \
	•	CNN on VAE-Reconstructed FGSM Data: Higher than direct FGSM (~80-90%) \
	•	GAN Discriminator: Scores closer to 0 for adversarial samples (fake)
