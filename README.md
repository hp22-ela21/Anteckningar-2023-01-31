# Anteckningar 2023-01-31
Demonstration av konvolutionellt neuralt nätverk (CNN) i Keras.

I filen "main.py" implementeras ett enkelt konvolutionellt neuralt nätverk bestående av 
tre konvolutionella lager, tre pooling-lager, ett flatten-lager samt två dense-lager.

Nätverket tränas under 10 000 epoker med färgbilder från datauppsättningen CIFAR-10, 
som innehåller bilder på bilar, båtar, hundar, katter, tåg med mera och normalt används
för att träna konvolutionella neurala nätverk. Efter träningen skrivs övergripande 
information om nätverket ut, exempelvis antalet parametrar med mera.

I filen "cnn.py" implementeras klassen dataset för enkel inläsning av träningsdata från
datauppsättningen CIFAR-10 via nedladdning från internet. En träningsfunktion definieras
också, som medför att de bästa parametrarna (vikterna och bias) sparas i en fil döpt
"model.weights.best.hdf5".