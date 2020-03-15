# Uge12: Biludlejning med Filer I/O og refaktorereing
### mandag d 16/3 - arbejder med biludlejning

### fredag d 13/3 - Java og filer - I/O

Mandag - læse biler ind fra filer og udskriv til fil
- opret fem klasser: Bil, Garage, ImportCarsFromFile, ExportCarsToFile og Main

### 1)cars1.csv I
Bil: lav konstruktør som svarer til headeren. 
ImportCarsFromFile: Lav en metode der tager en string som argument (filnavnet) og som bruger scanneren til at indlæse filen linje for linje. For hver linje skal den udskrive bilens Make og Model

Main: Instantiér ImportCarsFromFile og indlæs filen "cars1.csv"

### 1)cars1.csv II

Garage: Lav en konstruktør hvor garagen får et navn og hvor en liste til biler initialiseres
Garage: Lav en metode der kan sætte biler i garagen

ImportCarsFromFile: Du skal nu lave en bil for hver linje ved at splitte linjen. Bilen skal kun konstrueres vha Make og Model. Du skal altså lave en konstruktør i bil-klassen som gør dette muligt.

Main: Instantiér en garage som du sender med som parameter til ImportCarsFromFile (signaturen skal altså modificeres)

### 1)cars1.csv III

ExportCarsToFile: lav en metode der tager tre parametre - et filnavn, et filter og en Garage - som kan hente biler fra en garage og gemme de biler, som matcher filteret i en fil.
- det første filter skal være Volvo
- det andet filter biler som kører over 20 MPG
- det tredje filter biler som kører over 20 MPG eller har mindre end 200 HK

ImportCarsFromFile: Du skal nu tilføje en attribut - NumberOfDoors - som skal fiskes ud af model-betegnelsen. Så f.eks er "530i 4dr" en BMW med fire døre. Tag højde for de tilfælde hvor der ikke står noget om antallet af døre.


### 2)cars2.csv I
- cars2.csv

### 2)cars2.csv II

- cars3.csv
### 3)cars2.csv 
- cars4.csv

