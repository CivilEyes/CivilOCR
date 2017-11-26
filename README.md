# CivilOCR
CNN backed OCR for legal document of public elections

### Why
  To demonstrate semi-automated validation of public elections.

### Progress
  - [x] Load pdf files
  - [x] Checking layered and compressed images which are generated in latest versions of PDF files
  - [x] Simplifying complexed pdf images
  - [x] Extract images from pdf files
  - [x] Image postprocessing & binarization
  - [ ] Super resolution (backed by GAN)
  - [x] Noise reduction
  - [x] Table recognition
  - [x] Removing pen strokes between tables
  - [x] Table crop
  - [x] Table upright rotating
  - [x] Cell recognition
  - [x] Digit recognition
  - [ ] Multiple digit number recognition
  - [ ] Dashboard for table/graph output

### Data
  2017 presidential election of South Korea
  - Formally charged by and acquired from [National Election Commission](http://www.nec.go.kr)
  - Several raw data pdf files are bigger than github limit (50MB)
  - Thus there are limited number of files uploaded here. (14 areas in capital Seoul)
  - All raw data pdf files will be available under https://data.civiceyes.io
  - `filename_r.pdf` files are containing rasterized and simplified images rather than layered and complexed original images.
  - Rasterizing is done under Ubuntu system utilizing xdotool macros

### Image processing example
  ![example](/img/208,028.png)

### Prerequisites
  - [conda](https://conda.io)
  - Packages installable by `conda install`
    - [Python3](https://python.org)
    - [Jupyter iPython](https://ipython.org)
    - [Tensorflow](https://www.tensorflow.org)
    - [Keras](https://keras.io)
  - pillow with webp conversion
    - Install `libwebp-dev` and reinstall pillow with pip
  - xdotool for rasterizing (skippable)
