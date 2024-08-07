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
![7e floorplan with editor](https://github.com/user-attachments/assets/b57ad91c-1399-47a0-9cac-b3ed91bcdd9b)

![7d zoom view floorplan](https://github.com/user-attachments/assets/286bb747-acfb-4d29-a880-55a244dd2063)

![7c magic t cell view floor plan](https://github.com/user-attachments/assets/2629861f-45ea-445f-bb63-50c945663476)

![8a runplacement](https://github.com/user-attachments/assets/ff9dd21a-7c27-4897-beee-a69ea6bc5986)

![8b list of files in placement](https://github.com/user-attachments/assets/0dc959cd-b5f2-49b8-bd1a-2e2134cdd4d1)

![8c placement view](https://github.com/user-attachments/assets/28d1c5a2-8922-4314-90d4-a10cf9bf1e80)


![8d placement with command](https://github.com/user-attachments/assets/4690e305-33b8-4a9c-b62f-0a6bcc9388e5)

![8e placement zoom](https://github.com/user-attachments/assets/300137fb-fb38-4a59-976d-a9dd3c3e9808)

![9a IO change](https://github.com/user-attachments/assets/75154ab0-ffe2-44e1-81f7-9cc8ad1c4da5)

![9b after change layout](https://github.com/user-attachments/assets/084ecf42-5a11-4d9b-b197-350b0b2308c0)







4.Day3-Cell design using Magic Layout and Ngspice characterization.
--
![9c  cloning git hub](https://github.com/user-attachments/assets/bf77b52e-d3eb-4c51-b747-a45ba63e8eea)

![9d vsdstdcelldesign](https://github.com/user-attachments/assets/53638097-d6ca-4635-9fbb-497fb562de91)

![9d cmos inv](https://github.com/user-attachments/assets/8f68ad07-fbb2-4dee-b6c3-940fb7aff3f8)

![9f  run ngspice](https://github.com/user-attachments/assets/067bc6b2-b9f0-4630-ae51-b9cdaffa66ae)

![9f  extract all](https://github.com/user-attachments/assets/2f111efd-8c9a-438e-90f1-94f79d16c040)

![9g open spice file](https://github.com/user-attachments/assets/8f2cbc63-f2cb-4d5a-92db-72360ca751ef)

![9h plot](https://github.com/user-attachments/assets/a4867870-85de-41dd-9e12-2e95c18972bb)

![10a magic](https://github.com/user-attachments/assets/235923ed-edd1-46c4-91cc-77a07a8a6e0a)

![10b magic install](https://github.com/user-attachments/assets/09aad4fa-a399-43ed-98df-440625d3886d)

![10c](https://github.com/user-attachments/assets/963b0a4e-771e-4ac4-8023-4cdc9d984b3a)

![10d](https://github.com/user-attachments/assets/5c9aa518-20c5-4a4e-bcbd-abd38c7ea4ba)

![10e](https://github.com/user-attachments/assets/aa1f1c1a-c904-4b5e-a666-6788c92ea3f6)




5.Day4-Pre-layout timing analysis and importance to good clock tress(i.e minimum skewness).
--
![10g-lef file](https://github.com/user-attachments/assets/e5eff1bf-e479-4263-b299-2c42286aafbc)

![10f](https://github.com/user-attachments/assets/ac56484c-f4e3-4c34-9ef7-e900c2b81f07)


6.Day5-Final steps for RTL2GDS flow.
--

![final1](https://github.com/user-attachments/assets/a6851c61-7819-4cfd-b7f3-69f18fd60bce)


Running









