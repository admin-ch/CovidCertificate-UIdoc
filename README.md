# Web Management UI documentation

Documentation for the Web Management UI

# HOWTO create csv files for the csv upload function ?

## General information

The csv upload function allows you to create several certificates by importing a csv file. 

3 types of certificates can be created:
- vaccination
- test
- recovery

If you add [address information](https://github.com/admin-ch/CovidCertificate-Apidoc#address-data) in the csv file (only for vaccination and recovery certificates), then the files will be printed and sent per post directly to the certificate owner. 

The content of the csv is exactly the content needed by the API. Use the [API documentation](https://github.com/admin-ch/CovidCertificate-Apidoc#request---certificate-data) to be able to select appropriate values for the various fields of the csv file.

The csv separator is ;. It means that you can't use the ; in the columns of the csv file.

## Create a csv with excel

In order to put your data in a csv, we recommend to use Excel. You can follow the following steps:

1. Open one of the available excel template for [vaccination certificates](https://github.com/admin-ch/CovidCertificate-UIdoc/blob/main/template_vaccination.xlsx), [recovery certificates](https://github.com/admin-ch/CovidCertificate-UIdoc/blob/main/template_recovery.xlsx) or [test certificates](https://github.com/admin-ch/CovidCertificate-UIdoc/blob/main/template_test.xlsx)
2. Enter your data in the appropriate sheet. Information about format and valuesets can be found in the [API documentation](https://github.com/admin-ch/CovidCertificate-Apidoc#request---certificate-data)
3. In order to create a csv file, use the "File Save As" function and select the "csv" file type. Excel informs you that only one sheet can be exported since the csv format doesn't support several sheet. This is ok.
4. You can open the csv file with a text editor in order to check that everything is ok.
