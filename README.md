# Fingerprint Matching — Traitement d'image

Comparaison de deux empreintes digitales par traitement d'image et mesure de similarité structurelle (**SSIM**). Notebook réalisé dans le cadre d'un TP de traitement d'image.

![Python](https://img.shields.io/badge/Python-3-3776AB) ![Colab](https://img.shields.io/badge/Google-Colab-F9AB00)

## Pipeline

1. **Prétraitement** (Pillow) : niveaux de gris, redimensionnement 300×300, égalisation d'histogramme, binarisation (seuil 128) et détection de contours
2. **Comparaison** : score SSIM entre les deux empreintes (`scikit-image`)
3. **Décision** : empreinte **acceptée** si SSIM ≥ 0,75, **rejetée** sinon
4. **Visualisation** des deux images prétraitées (Matplotlib)

## Lancer

Ouvrir le notebook dans Google Colab ou Jupyter, puis charger deux images d'empreintes.

```bash
pip install numpy pillow scikit-image matplotlib
```

## Technologies

Python · NumPy · Pillow · scikit-image · Matplotlib
