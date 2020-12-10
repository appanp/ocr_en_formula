This repo has scripts to do image character recognition (a.k.a OCR) which also has formulas.

This OCR is designed & tested to process only the text image with following restrictions:

1. Only typed text images, no hand-written images.
1. Can have mathematical formulas mixed with text.
1. Can have figures mixed with text but figures are not further processed.

### Input Image Processing Pipeline

TODO: Add more details, but at a high-level, it consists of the following:

1. **Image Segmentation**: Input image segmentation into regions which has only text, figures and mathematical formulas.
    * This is kind-of high-level parsing of images into its components.
    * Text component does not have any formatting text like bullets, numbers, etc.
1. **Component Processor*: Each identified sub-image is processed by specific component processor.
