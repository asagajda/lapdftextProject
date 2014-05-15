lapdftextProject
================

High-level build project for all LAPDF-Text submodules.

*Note* - we have currently deprecated the development of the LA-PDFText rule web application that is not tied to the digital library. This means that we will no longer be developing the [lapdftextServer](https://github.com/BMKEG/lapdftextServer) web application separately of the [sciKnowMine](https://github.com/BMKEG/sciKnowMine) system. Interested developers and users are referred to the [sciKnowMineProject](https://github.com/BMKEG/sciKnowMineProject) for more information. 

To run this project, you should be able to compile this system directly from the download. This project is now *only* concerned with the [lapdftext](https://github.com/BMKEG/lapdftext) library, which is the base level
library containing all functionality for directly interacting with PDF files through the 
use of the JPedal GPL open source library (Beta level of development). 

To run the LA-PDFText library from source:

   git clone https://github.com/BMKEG/lapdftextProject
   git submodule update --init --recursive
   mvn -DskipTests clean package 
   cd lapdftext
   mvn -DskipTests assembly:assembly
   
This will generate a file `lapdftextProject/lapdftext/target/lapdftext-1.7.4-SNAPSHOT-jar-with-dependencies.jar` that you may then use to run commands:


   
