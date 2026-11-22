# Pham Minh Tung

Semiconductor IC Design student at FPT University, Ho Chi Minh City.
I write synthesizable Verilog, verify it against bit-exact Python golden models, and report what Vivado says about area and timing.

**Portfolio** [ygbzyem.github.io/my-portfolio](https://ygbzyem.github.io/my-portfolio/) · **LinkedIn** [tung-pham-a33761420](https://www.linkedin.com/in/tung-pham-a33761420/) · **CV** [PDF](https://ygbzyem.github.io/my-portfolio/assets/pdf/Resume.pdf)

## Selected projects

| Project | What it is | Results |
|---|---|---|
| [3×3 Image Convolution on FPGA](https://github.com/Ygbzyem/FPGA_RealTime_Conv3x3_Processor) | Streaming blur/sharpen pipeline, built as an adder tree and as a 9-PE systolic array | 181–187 MHz in Vivado · systolic uses 2.3–2.9× the LUTs · 97–99 % of pixels match the golden model |
| [Pipelined AM Modulator](https://github.com/Ygbzyem/AM-Modulation) | Two 32-bit NCOs, Q11 fixed-point datapath, full- vs quarter-wave sine ROM | Quarter-wave ROM: 29 % fewer LUTs, 133.5 MHz · 18/18 regression cases bit-exact |
| [TDM Multiplexer / Demultiplexer](https://github.com/Ygbzyem/TDM-4---Channel-Multiplerxer-Demultiplexer) | Parameterized N-channel, W-bit link timed by one counter, no FSM | 22 LUT · 64 FF on Kintex-7 · timing met at 100 MHz · 200/200 random vectors |
| [Offline Keyword Spotting on ESP32](https://github.com/Ygbzyem/AI-Keyword-Spotting-With-ESP32) | 22-class 1D-CNN running on our own ESP32 board with an I2S microphone | 91.2 % validation accuracy · int8 model in 136 KB flash |
| [Line-Following Robot](https://github.com/Ygbzyem/Robot-Line-Follower-Obstacles-Detector) | ESP32-S3 line-maze robot for the F-Chip contest | 8-channel line sensing · encoder speed control · VL53L0X obstacle avoidance |

## How I work

- Spec first: port tables, widths and latency written down before RTL.
- A Python golden model and a self-checking testbench for every RTL design.
- Numbers from post-implementation reports, with known limitations written down.

## Tools

- **HDL & languages:** Verilog · SystemVerilog (basic) · Python · C/C++ · Tcl
- **EDA & hardware:** Vivado · ModelSim · Icarus Verilog · KiCad · LTspice · ESP32
- **Workflow:** Git · Linux

## Now

- Comparing accumulator architectures for the 3×3 convolution core.
- Starting FPGA labs on an EBAZ4205 (Zynq-7010) board.
