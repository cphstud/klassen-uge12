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

Bil: Du skal ændre i konstruktøren så den laver en løbende id (brug en statisk attribut som tæller)

Bil: Du skal ændre i konstruktøren endnu engang så den løbende id kommer fra en hjælpeklasse der har en statisk attribut som tæller og en statisk metode - getCarId() - som du kan kalde fra din konstruktør

### 2)cars2.csv I
#### Der er nu kommet flere biler og flere attributter
Garage: Du skal tilføje en id til konstruktøren (bruge en statisk tæller)
Bil: Du skal ændre i konstruktøren så den kan lave biler med de attributter som fremgår af headeren. Du skal desuden tilføje en attribut hvor garagens id kan sættes (og gettes)
ImportCarsFromFile: Du skal nu ændre i signaturen så den modtager filnavn samt returnerer en arrayliste af garager. Hver garage skal fyldes med 20 biler og hver bil skal stemples med garageid'et (hint:modulus)
CarHandler: Du skal lave en ny klasse som har en metode - findCarGarageByReference - som modtager en reference samt listen af alle garager. Den skal returnere en bil. Metoden skal kaste en exception hvis den finder mere end én bil. Lav en testfil som kan fremprovokere denne fejl


### 3)cars2.csv 
Vi mangler el-biler. De kan findes i denne fil.
- cars4.csv

