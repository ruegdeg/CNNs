# Edge detection on remote sensing imagery

Using this repo you can builds and runs an container and run an edge detection using the DexiNed-Pytorch https://github.com/xavysp/DexiNed/tree/master/DexiNed-Pytorch

To train and test the model we combined a set of 104 image tiles of 1280X780 px taken from orthophotos of 0.1m resolution with a corresponding tiles outlining the edges of agricultural fields. The later was taken from agricultural land use dataset of Switzerland. The allocation of the tiles was cafefully selected to ensure that the content of both dataset match together (does not to have to be the case in overall) 

To run smooothly the train/test we suggest you to install the Singularity https://sylabs.io/docs/ which is a container platform. You  can then simply download the container from [this GGDrive location](https://drive.google.com/drive/folders/1wui0kZRPNZ8feZVq0CU2GIn7XJhrORpz?usp=sharing)  and launch the edge detection algorithms using e.g., this command:

singularity shell -B PATHtoYOURlocationOFtheDEXINED Python37_DexinetPytorch_v2.sif 

and then running the script using 

python main.py --input_dir=PATHtoYOURlocationOFtheDEXINEDedgeFILES

