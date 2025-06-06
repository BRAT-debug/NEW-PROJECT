# PlantPal: AI Plant Health Monitor

Final project for the Building AI course

## Summary

PlantPal is an AI-powered app that helps users monitor the health of their houseplants by analyzing leaf images to detect diseases, pests, or nutrient deficiencies. It provides care tips to keep plants thriving.

## Background

Houseplant care is increasingly popular but many people struggle to identify early signs of plant stress or disease. Common problems include:
* Misdiagnosing plant diseases and pests
* Over- or under-watering due to lack of feedback
* Difficulty in identifying nutrient deficiencies

This project aims to make plant care accessible, reduce plant loss, and increase user confidence in gardening.

## How is it used?

Users simply take a photo of their plant’s leaves with their smartphone. The AI model analyzes the image and returns:
* Possible diagnoses (disease, pest, deficiency)
* Severity level
* Personalized care instructions (watering, light, treatment)

It’s useful for home gardeners, office plant caretakers, and plant shops. The app can be used anytime a user suspects a plant is unhealthy or just for routine checkups.

![PlantPal Screenshot](https://example.com/plantpal_screenshot.png)

```python
def diagnose_plant(image):
    # Load image and preprocess
    processed_img = preprocess(image)
    # Predict disease or deficiency
    diagnosis = model.predict(processed_img)
    return diagnosis
## Data sources and AI methods

Plant images and disease labels were collected from publicly available datasets such as PlantVillage. We use a convolutional neural network (CNN) trained on thousands of leaf images for classification.

| Syntax       | Description                                             |
|--------------|---------------------------------------------------------|
| CNN          | Convolutional Neural Network for image classification   |
| Preprocessing| Resizing, normalization, and augmentation of images     |

## Challenges

* Limited dataset diversity may reduce accuracy on rare plants or diseases.
* The app cannot replace expert botanical advice for complex cases.
* Ethical considerations include privacy of user-uploaded images and responsible usage advice to avoid misuse of chemicals.

## What next?

Future work could include:

* Expanding the dataset with user-contributed images to improve model accuracy.
* Adding pest detection using video input.
* Multilingual support for global accessibility.
* Integration with smart watering devices for automated plant care.

## Acknowledgments

* Inspired by PlantVillage dataset and research community
* Model architecture based on open-source CNN implementations
* Image: Plant Leaf by John Doe / CC BY 4.0
