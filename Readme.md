## ACM Grand Challenge on Cheapfakes Detection (2023)

Developed a Flask application for fake news detection, specifically targeting cheapfakes (miscontextualization).

## Dataset(COSMOS):
- Train: 160K images, 360K captions
- Validation: 40K images, 90K captions
- Test: 1700 images, 3400 captions (with context annotations)

## Key Features
- Binary classification: OOC (label 1) or Not OOC (NOOC, label 0).
- Input: Image with two captions.
- Multi-modal analysis combining image and text.
- Ensemble model technique for classification.
- Context-aware image representation learning.


## Getting Started
1. Clone the repo: `git clone https://github.com/simR122/final_rep.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Download the dataset using the provided script
4. Visualize data: `python dataset_visualizer/visualize.py`
5. Train and test for image-text matching:
   - Set up Detectron2 following [official instructions](https://detectron2.readthedocs.io/en/latest/tutorials/install.html)
   - Configure `utils/config.py`
   - Train: `python trainer_script.py -m train`
   - Evaluate: `python trainer_script.py -m eval`
6. Test for out-of-context detection: `python evaluate_ooc.py`

**For detailed instructions**, refer to the (https://detecting-cheapfakes.github.io/icmr-2024.html).







