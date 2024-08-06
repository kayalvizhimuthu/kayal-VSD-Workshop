#VSD-Workshop
------          
------             
**Contents**
---
1.Introduction

2.Day1-Introduction to open source eda tool(openlane) and PDK(skywater130nm) and synthesis of RTL

3.Day2-Floorplan and Powerplan.

4.Day3-Cell design using Magic Layout and Ngspice characterization.

5.Day4-Pre-layout timing analysis and importance to good clock tress(i.e minimum skewness).

6.Day5-Final steps for RTL2GDS flow.

1.Introduction
--
OpenLane is an open-source ASIC (Application-Specific Integrated Circuit) flow that facilitates the design and implementation of digital integrated circuits. It provides a complete RTL-to-GDSII (Register Transfer Level to Graphic Data System II) flow, leveraging various open-source EDA (Electronic Design Automation) tools. Developed by Efabless Corporation.

2.Day1-Introduction to open source eda tool(openlane) and PDK(skywater130nm) and synthesis of RTL
--
step1:Open linux terminal and use various linux commands
![1  use linux commands](https://github.com/user-attachments/assets/00236cb8-6780-4443-95e5-386cf41a65cf)



1. cd : It is used to change the current working directory.
   
2. ls : It lists the contents of a directory.
   
3.ls -ltr : It lists the contents of a directory 

4.ls --help: It displays a help message with a list of options and usage information for the "ls" command. 

5.clear: It clears the terminal screen.

linux commands for working dirctory forthis workshop

1.cd Desktop 

2.cd work/tools/ 

3.cd openlane_working_dir/

4.cd openlane/

![2 openlane directory structure](https://github.com/user-attachments/assets/35430ea7-b48e-478b-82fc-0d18cc5c48af)


step2: setting upopenlane environment

After openlane type PDK it open bash, then to enter followingcommands

docker

./flow.tcl -interactive

package require openlane 0.9

prep -design picorv32a

![3 design preparation](https://github.com/user-attachments/assets/41b28c69-afb4-4ee8-a21d-75037a702544)

step3:Synthesis of the RTL

run_synthesis

![5  synthesis completion](https://github.com/user-attachments/assets/f5fad124-4a9f-463f-806c-9ff814b6b8f1)

step4:Calculate the flop ratio

![6 calculate flopratio](https://github.com/user-attachments/assets/46b81cbc-4293-4a8a-9e0d-5036518bf3da)


3.Day2-Floorplan.
--

step1: Running floorplan

run_floorplan

![7  run floorplan](https://github.com/user-attachments/assets/dabf61c3-9d9a-440b-9092-9c892fa514fd)

step2:Magic layout view



4.Day3-Cell design using Magic Layout and Ngspice characterization.
--


5.Day4-Pre-layout timing analysis and importance to good clock tress(i.e minimum skewness).
--


6.Day5-Final steps for RTL2GDS flow.
--
Running









