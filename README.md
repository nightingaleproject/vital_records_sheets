# Vital Records Sheets
This repo contains the master copies of the IJE and Forms spreadsheets used to generate Structure Definition Intros, IJE Mapping Pages, and Forms Mapping Pages in VRCL, VRDR, and BFDR IG's. 

Scriptology for generating the structure definition intros or mapping pages pull from this repo to include the latest versioning of the spreadsheets. Therefore, any lasting changes to content in the spreadsheets should be made here, and not locally in the IG.   

The two CSV Files that drive generation of content and should be edited are:
* IJE/FHIR Mapping - [csv](IJE_File_Layouts_and_FHIR_Mapping_24-06-21.csv).
* Forms Mapping - [csv](Forms_Mapping.csv)

The xlsx files are historical or derivative, and should not be directly edited:
* Historical FHIR/IJE Mapping (xlsx)()
* Generated FHIR/IJE Mapping (xlsx)() -- this is generated from the [master CSV File](IJE_File_Layouts_and_FHIR_Mapping_24-06-21.csv) by running the [makeExcelFromCSV.rb](makeExcelFromCSV.rb) script.

To create the derived xlsx file run:  ruby makeExcelFromCSV.rb 
You may need to run: gem install write_xlsx




