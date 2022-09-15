# GRETINA
This anonymous repo is created to support RR for the GRETINA dataset during the blind-review process of the paper. 



Use the following code to generate images:

From "https://github.com/NVlabs/stylegan2-ada-pytorch", use SG2_ADA Pytorch code and run the following line

!python generate.py --outdir="Your prefered directory" --trunc=0.7 --seeds=1-5000000 \
    --network="directory in which the pickle file network-snapshot-000120 is saved.pkl"
