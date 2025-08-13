# IIR-xilinx
Academic project for the course of Embedded Computing Systems. The aim of the project was to design and implement an IIR audio filter on FPGA
## Aim
Design a digital circuit which implements a simple IIR filter for audio applications

y[n] = y[n-1] - 0.25·x[n] + 0.25·x[n-4]

Such filter allows to attenuate signal components which have half the frequency of the sampling one.

Refer to a possible 16-bit wav format.

## Tools
The tools used for the project were
* [MATLAB R2021a](https://it.mathworks.com/products/matlab.html) for modeling
* [Active-HDL Student Edition](https://www.aldec.com/en/products/fpga_simulation/active_hdl_student) for VHDL implementation and testbenches
* [Vivado HLx Edition 2020.1](https://www.xilinx.com/products/design-tools/vivado.html) for synthesis on FPGA

## Project structure
The project folder resembles the following structure:

* matlab: MATLAB design files
* db
  * src: VHDL source files
  * tb: VHDL testbench files
* active_hdl: Active-HDL project folder
* vivado_synth: Vivado project folder

The design workflow can be found in the [report](https://github.com/gabrielebaris/IIRAudioFilterFPGA/blob/master/report/report.pdf) file.
