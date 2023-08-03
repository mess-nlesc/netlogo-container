# netlogo-container
Apptainer/Singularity container for netlogo
## Build
Build needs a Linux system with sudo rights.
```
./build.sh
```
## Test
Run one of the examples provided by netlogo as a test.
```
./run.sh
```
## Run your own model in headless mode
```
apptainer exec netlogo.sif netlogo-headless.sh --model "PATH TO MODEL IN YOUR HOME DIR" --experiment "EXPERIMENT NAME" --table OUTPUT.CSV
```
