# Detection of motor endplates using ultrafast ultrasound
[![GitHub stars](https://img.shields.io/github/stars/luuleitner/MotorEndplate?label=Stars&style=social)](https://github.com/luuleitner/MotorEndplate)
[![GitHub forks](https://img.shields.io/github/forks/luuleitner/MotorEndplate?label=Fork&style=social)](https://github.com/luuleitner/MotorEndplate)
<br>
[![License: Apatche-2](https://img.shields.io/hexpm/l/plug)](https://www.apache.org/licenses/LICENSE-2.0)
[![GitHub contributors](https://img.shields.io/badge/Contributions-Welcome-brightgreen)](https://github.com/luuleitner/MotorEndplate)

<p align="center">
<img src="https://github.com/luuleitner/MotorEndplate/blob/master/figures/contraction.gif">
</p>

# Repository Structure

This repository provides code and datasets for ultrafast ultrasound investigations on an electrically stimulated medial gastrocnemius muscle.

### 1. Code
- `MotorEndplate\functions` folder includes the used functions (eg. Butterworth lowpass filter)
- `MotorEndplate\SPTtracker.m` is the Matlab script to execute sampling point tracking. This program will return the sampling point coordinates along a chosen facile line for each investigated timestep.
- `MotorEndplate\MEP_extraction.ipynb` is Jupyter notebook for MEP extraction. The script inputs filtered x and y displacements (as .csv files) and outputs starting time of the contraction for each sampling point. To run the script, please, meet the requirements listed below.

### 2. Requirements
- For Python code please use the version 3.6.1 of the interpreter and install all the packages listed in `requirements.txt`.

### 3. Dataset
The high frame rate ultrasound recording (1500 Hz) of an electrically stimulated medial gastrocnemius contraction can be downloaded from: [google drive](https://drive.google.com/file/d/1UnxKz-48edv91yl6tduEGyUoVwtJ64Iq/view?usp=sharing) (679 MB). The provided dataset (`MGcontraction.avi`) is licensed under a [Creative Commons Attribution 4.0 International License](https://github.com/luuleitner/MotorEndplate/blob/master/license/LICENSE_dataset).

[![CC BY 4.0](https://i.creativecommons.org/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)

### 4. Add-On's
- We used `pybf` to reconstruct ultrasound images from radio frequency data. This python based delay-and-sum beamformer is available for open-sorce use here: [pybf](https://github.com/Sergio5714/pybf)
- `MotorEndplate\figures` folder includes all result plots and figures of the IEEE-IUS 2020 publication in high resolution.

# Credits

"do, ut des"...if we could assist you with this code and dataset please cite our work:
```
@inproceedings{Leitner2020,
   title={{Detection of Motor Endplates in Deep and Pennate Skeletal Muscles in-vivo using Ultrafast Ultrasound},
   author={Christoph Leitner and Sergei Vostrikov and Harald Penasso and Pascal A. Hager and Andrea Cossettini and Luca Benini and Christian Baumgartner},
   booktitle={in Proc. of the IEEE International Ultrasonic Symposium},
   venue={Las Vegas,USA},
   publisher={IEEE},
   month=09,
   year={2020}  
}
```

# License

This program is free software and licensed under the Apache License 2.0 - see the [LICENSE](https://github.com/luuleitner/MotorEndplate/blob/master/license/LICENSE_code) file for details.

