# GRETINA
This anonymous repo is created to support RR for the GRETINA dataset during the blind-review process of the paper. 


The file "Discarded_left_samples.csv" contains the list of 42 Messidor-2 samples that we discarded from Messidor-2 data set.

Link to the training set: https://drive.google.com/file/d/1c5-kQFHRtAa4yEHEG-_5mPOg_m2iKLpw/view?usp=sharing

Here is the link to the shared folder that contains the generated retina images that we used for unlinkability evaluation. We resized them to 750x750 pixel images before using. Link: https://drive.google.com/drive/folders/1HELUM4FBz85LisCEQFdg_iHRWOnpSGgw?usp=sharing

Here is the link to the snapshot for 5,000,000 generated retina. Use the pickle file to generate the retinal images. Link to the trained model: (https://drive.google.com/file/d/1LYsNTU-g23k0wNWeYzDdADkafIuyhM0D/view?usp=sharing)

Note: --trunc=0.7 will generate 70% of the images which have better quality.
Use the following code to generate images:

From "https://github.com/NVlabs/stylegan2-ada-pytorch", use SG2_ADA Pytorch code and run the following line

!python generate.py --outdir="Your prefered directory" --trunc=0.7 --seeds=1-5000000 \
    --network="directory in which the pickle file network-snapshot-000120 is saved.pkl"
