# Edge detection on remote sensing imagery

Using this repo you can builds and runs an container and run an edge detection using the DexiNed-Pytorch https://github.com/xavysp/DexiNed/tree/master/DexiNed-Pytorch

To run smooothly we suggest you to install the Singularity https://sylabs.io/docs/ which is a container platform. You  can then simply download the container from [this GGDrive location](https://www.google.com)  and launch the edge detection algorithms using e.g., singularity shell -B PATHtoYOURlocationOFtheDEXINED Python37_DexinetPytorch_v2.sif and then running the script using python main.py --input_dir=PATHtoYOURlocationOFtheDEXINEDedgeFILES

