# cs230 project - Offline handwritten mathematical expression to LaTeX conversion
1) Uses data from the Mathwriting dataset from Google (https://arxiv.org/abs/2404.10690)
2) mathwriting_explore_data.ipynb - Colab notebook to explore data excerpt, display some of the images and annotations
3) process_data_inkml_to_rgb.ipynb - Convert inkml data for images of different sizes in the mathwriting dataset to (128, 256) images and save to RGB files
4) process_data_inkml_to_rgb_annotations.ipynb -  Same as (3) + also save LaTeX annotations to files. Data is save in Google Drive as explained in the report and in the colab files
5) HME_StageA_CNN.ipynb - Reads in training images (X) and corresponding LaTeX labels (Y) and feeds them to a CNN, which generates features to be fed to Stage B (encoder) -> Stage C (decoder). They stages will be combined to form the full model.
6) HME_StageABC.ipynb - Adds encoder/decoder stage to the CNN (partial)
