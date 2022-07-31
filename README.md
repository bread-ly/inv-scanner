# bread-ly.github.io
This is a website for my diploma thesis.
We created an inventory-scanner for the local fire brigade.

# Dependencies
The application uses the https://github.com/mebjas/html5-qrcode Barcode Reader.
It is also using the https://github.com/parallax/jsPDF PDF Creation tool.
# Data-file
For the Data File we use JSONp whith the following format.

data='[{"invInvNummer":"8/13","invName":"sample1","raumName":"room1","mitNr":"0","mitVorname":"","mitNachname":"","invBaujahr":"2022","invPrüfPflichtig":"-"}

This file is initialized by scanning a QR-code with the link to the raw file.

# Insctruction/Initialization
Create PDF:
For the creation of the PDF jspdf is used, i made a class for simlper access.
When creating the object, hand over the x coordinate that the text is printed at, the space beetween two collumns and the Organisation name for the PDF-head.
const pdf = new PDF(x-coordinate, collumnspace, organisation);
