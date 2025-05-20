# A Novel Study on Deep Learning Based Adversarial Attack Techniques on Digit Recognition

## Overview

This project presents a comparative analysis of four adversarial attack techniques—**FGSM, BIM, JSMA, and C\&W**—on the MNIST digit recognition task using CNNs.

## Motivation

Despite high accuracy, neural networks remain vulnerable to small, imperceptible input perturbations. This study explores the severity of that vulnerability through popular adversarial techniques.

## Dataset

Experiments were conducted on the **MNIST dataset**—a standard benchmark of 60,000 training and 10,000 test grayscale digit images.

## Attack Methods

* **FGSM**: Single-step gradient-based perturbation. Fast but less effective.
* **BIM**: Iterative version of FGSM, with improved attack success.
* **JSMA**: Uses saliency maps to selectively modify key pixels.
* **C\&W**: Optimizes adversarial loss to create highly effective, subtle attacks.

## Evaluation Metrics

Attacks were compared using:

* Accuracy on adversarial examples
* Prediction probability drop
* Successful attack rate
* Confidence reduction

## Key Findings

* **FGSM** had limited success.
* **BIM** and **JSMA** were more effective, lowering accuracy significantly.
* **C\&W** was most potent, achieving 100% success and 0% model accuracy on adversarial samples.

## Security Implications

Results highlight the need for robust ML defences like adversarial training, gradient masking, or defensive distillation—especially in safety-critical applications.

## Applications

Findings are relevant to adversarial risks in domains like:

* Finance (fraud detection)
* Healthcare (medical diagnostics)
* Autonomous vehicles
* Cybersecurity
* Biometric systems

## Future Work

Potential directions include testing advanced attacks (e.g., PGD, MIM), enhancing defences, and generalizing to broader datasets (CIFAR-10, ImageNet, IMDB).

## Conclusion

The study underscores deep learning's vulnerability to adversarial manipulation, with **C\&W** proving most damaging. Robust defence strategies are critical for safe deployment.

---

## Citation

If you use this code in your work, please cite:

```bibtex
@INPROCEEDINGS{10859499,
  author={Mathew, Joel Stephen and Balachandra, Anumaneni Venkat and Nair, Aditya Suresh and Bhati, Arman Singh and Mohana and P, Ramakanth Kumar},
  booktitle={2024 9th International Conference on Communication and Electronics Systems (ICCES)}, 
  title={A Novel Study on Deep Learning Based Adversarial Attack Techniques on Digit Recognition}, 
  year={2024},
  pages={2070-2076},
  doi={10.1109/ICCES63552.2024.10859499}}
```
