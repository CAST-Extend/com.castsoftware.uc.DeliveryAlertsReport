# 1. Description

This Extension should be useful in the following situations:
* The source code provided is incomplete or requests the installation of thirdy party frameworks or libraries;
* There is a large number of applications in the delivery folder;
* The source code is extracted from repositories (TFS, SVN,...) that have been populated from external suppliers;
* There is the need to analyze with CAST AIP all the source code provided in the delivery folder;
* There is the need to compile and/or deploy the applications in the delivery folder;
* The customer needs to know if the sources delivered by the suppliers are complete or missing of some files or libraries needed for compile and/or deploy the applications (ex. for changing suppliers).

## 1.1 How to use it

The Extension is an executable program provided with two interfaces: Windows Forms and Command Line.

The Windows Forms Tool can be lauched from the executable file DeliveryAlertsReport.exe and looks like this:

![](https://github.com/CAST-Extend/com.castsoftware.uc.DeliveryAlertsReport/blob/master/Form.png?raw=true)

The "CAST AIP Delivery Folder" parameter must point to the root of the CAST AIP Delivery Folder:

![](https://github.com/CAST-Extend/com.castsoftware.uc.DeliveryAlertsReport/blob/master/Form2.png?raw=true)

With the "Report Path" parameter It is possible to select the output path for the Excel Report produced by the tool (*.xlsx)

The creation of the report will start after pushing the "Generate Report" button.
There will be displayed a log in the "Log" box for all the operations until the completion of the report:

![](https://github.com/CAST-Extend/com.castsoftware.uc.DeliveryAlertsReport/blob/master/Form3.png?raw=true)

There is also the possibility to use the Command Line interface (i.e. for automation):

Usage: DeliveryAlertsReport-CLI.exe \<DeliveryFolder\> \<ExcelReportPath\> \<LogFilePath\>

## 1.2 Output

The output produced is an Excel report:

![](https://github.com/CAST-Extend/com.castsoftware.uc.DeliveryAlertsReport/blob/master/Report.PNG?raw=true)

For each alert raised by DMT for each application in the Delivery folder in the latest version delivered, here is provided:
* Name of the application 
* Date of the latest version
* Path of the project that references the missing file
* Name or Path of the missing file referenced by the project (for DLLs or Jars is provided the name of the library, for missing source files is provided even the path where the file is expected)

# 2. CAST AIP Compatibility

The following table gives the list of CAST AIP configurations where the Extension has been implemented:

* CAST AIP 8.0.x
* CAST AIP 8.1.x
* CAST AIP 8.2.x

# 3. Prerequisites & Installation

## 3.1 Prerequisites

The following table gives the complete list of technical prerequisites to be met before installing the Extension:

* An installation of any compatible release of CAST AIP (see table above)
* MS .Net Framework v.4.5.2

## 3.2 Installation Instructions

The extension is ready after downloading it in the download folder, without need of any installation.

