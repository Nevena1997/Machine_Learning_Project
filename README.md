# Face Mask Detection - Detekcija lica sa maskom 

Ovaj projekt je rađen u sklopu predispitnih obaveza na kursu Mašinsko učenje na master studijama.

Ideja projekta je konstrukcija detektora zaštitne maske koji bi na video snimku prepoznao lice (bilo sa maskom ili bez nje), a potom ga uokvirio i ispisao odgovarajuću poruku, u zavisnosti od toga da li se na licu nalazi zaštitna maska. Opisana ideja je realizovana kroz više faza: (sad ćemo ovde ispod da metnemo neku sliku).

Za prepoznavanje lica u prvom koraku korišćen je cascade classifier (sad neko fensi objašnjenje šta je to) iz biblioteke cv2 (je l tako?). Slika lica izdvojenog primenom ovog klasifikatora se uz odgovarajuće korake pretprocesiranja (pišemo dole o tome) prosleđuje konvolutivnoj neuronskoj mreži koja će dati predikciju o tome da li se na licu nalazi maska ili ne. (Sad sledi opis onog dela kad se lice uokviri nekom bojom i ispisuje se odgovarajuća poruka, ovo ne umem baš lepo da objasnim još uvek xD).

Trenažni i validacioni skup slika (__train__ i __valid__, redom) korišćeni prilikom obučavanja mreže i njene evaluacije preuzeti su sa sajta https://www.kaggle.com/ashishjangra27/face-mask-12k-images-dataset (baci samo pogled je l si odavde preuzela slike hahah).

## Pretprocesiranje

Pre nego što utreniramo mrežu nad slikama iz skupa __train__, svaku sliku ćemo konvertovati u grayscale (kako ovo na srpskom lepo da napišem?), a potom i promeniti njenu dimenziju na 100x100. Kako bismo ubrzali prcoes treniranja mreže, slike ćemo dodatno i normalizovati, odnosno svesti vrednosti njihovih pojedinačnih piksela na vrednosti iz intervala [0,1].

## Treniranje mreže

## Evaluacija
#### Cascade Classifier
