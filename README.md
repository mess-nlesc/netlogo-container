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
apptainer exec netlogo-headless.sif netlogo-headless.sh --model "PATH TO MODEL IN YOUR HOME DIR" --experiment "EXPERIMENT NAME" --table OUTPUT.CSV
```
Or use the container executable directly to run the model. N.B. you need to escape the quotes in this example.
```
./netlogo-headless.sif --model \'/app/netlogo/models/IABM Textbook/chapter 4/Wolf Sheep Simple 5.nlogo\' --experiment \'Wolf Sheep Simple model analysis\' --table wolf_sheep_output.csv
```
