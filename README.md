=======================================================================
# Gamut Installer
=======================================================================


## 1. Download Gamut Installer (372MB - Contains MongoDB, Wildfly Server and sample vcf data) 

    https://drive.google.com/uc?id=1NCN1lOhz16U8433e7lbvWjq6EDtVvOEc&export=download
    
    **Using Wget Command**
        export fileid=1NCN1lOhz16U8433e7lbvWjq6EDtVvOEc
        export filename=gamut.zip
        wget --save-cookies cookies.txt 'https://docs.google.com/uc?export=download&id='$fileid -O- | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1/p' > confirm.txt
        wget --load-cookies cookies.txt -O $filename 'https://docs.google.com/uc?export=download&id='$fileid'&confirm='$(<confirm.txt)
   
## 2. Copy into New Directory  
   
    mkdir gamut
    mv gamut.zip gamut/
    cd gamut/
    
## 3. Unzip  
   
    unzip gamut.zip  
   
## 4. Run Gamut   
    
    ./gamut.sh

## 5. Open into the Browser
    
    http://localhost:8080/

## Demo
![Gamut_Installer](https://raw.githubusercontent.com/Bioinformatics-Group-C-DAC/GamutInstaller/master/gamut.gif)