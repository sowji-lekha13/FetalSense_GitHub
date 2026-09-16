# FetalSense - Official GitHub Page

This is the project page for **FetalSense: Anatomy-Guided Fetal–Probe Motion Disentanglement in Freehand Ultrasound**, built on data engineered by the companion dataset paper **FLAME-US**.

Built from the [UltraGym_Blog](https://github.com/Ragu2399/UltraGym_Blog) template.

## Paper Information

- **Title**: FetalSense: Anatomy-Guided Fetal–Probe Motion Disentanglement in Freehand Ultrasound
- **Authors**: Sowjanya Balaji, Anusha A, Keerthi Ram, Shyam Ayyasamy, Suresh Seshadri, Manojkumar Lakshmanan, Mohanasankar Sivaprakasam
- **Dataset paper**: FLAME-US: A Landmark-Guided Dataset for Quantitative Fetal Motion Analysis in Freehand Ultrasound

## Abstract

Fetal movement is an important indicator of fetal well-being and underpins routine obstetric ultrasound (US) tasks such as biometric assessment and standard-plane acquisition. Accurate motion estimation is therefore essential for both clinical analysis and autonomous US systems. However, anatomical changes observed in freehand US image sequences arise from the combined effects of fetal and probe motion, creating a motion ambiguity that makes fetal-motion estimation inherently ill-posed. To address this challenge, we introduce FetalSense, a framework for disentangling fetal and probe motion from US image pairs. FetalSense is trained using simulation-derived SE(3) pose supervision for both the fetus and probe, while requiring only US images and tracked probe motion at inference. We further introduce Anatomical Landmark Displacements (ALDs), an image-derived signal of fetal motion based on temporal changes in fetal anatomy, thereby providing supervision without requiring fetal-pose measurements at deployment. FetalSense combines a probe-pose-conditioned image encoder with an ALD-guided landmark stream to enable explicit motion decomposition. FetalSense achieves a mean fetal displacement error of 1.56 mm and a decomposition closure error of 0.69 mm, and its learned fetal-motion representation supports motion-state classification at 94.1% accuracy and 96.7% F1-score.

## File Structure

```
.
├── index.html              # Main page
├── css/
│   └── style.css           # Shared stylesheet (from the UltraGym_Blog template)
├── images/
│   ├── fig1_architecture.jpg          # FetalSense architecture (Fig. 1)
│   ├── fig2_motion_decomposition.jpg  # Motion decomposition analysis (Fig. 2)
│   ├── fig3_motion_state.jpg          # Motion-state classification (Fig. 3)
│   ├── flame_us_pipeline.jpg          # FLAME-US dataset curation pipeline
│   ├── flame_us_correlation.jpg       # ALR vs. fetal-rotation correlation
│   └── flame_us_alr_qualitative.jpg   # Qualitative static vs. moving ALR behaviour
├── paper.pdf                 # FetalSense camera-ready PDF
└── flame_us_paper.pdf        # FLAME-US dataset paper PDF
```

## To Publish on GitHub Pages

1. Push this folder's contents to a GitHub repository.
2. In the repo settings, enable **GitHub Pages** for the `main` branch (root).
3. Your page will be live at `https://<username>.github.io/<repo-name>/`.

## To Do Before Publishing

- [ ] Confirm the target venue/conference and replace the "Preprint" label in `index.html` and the BibTeX entries.
- [ ] Add a code/dataset release link once available (currently noted as "to be released" in the paper text).
- [ ] Double-check author emails and affiliations in the footer.
