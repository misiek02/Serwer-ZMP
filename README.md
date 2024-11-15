# Serwer-ZMP
Serwer do wizualizacji 3D

#Skorzystanie z niniejszego oprogramowania wymaga zainstalowania
 - biblioteki SOIL (pakiety: libsoil-dev, libsoil1)
```sh
sudo apt install libsoil-dev
```
```sh
sudo apt install libsoil1
```

#Domyślnie aplikacja kompiluje się z wykorzystaniem biblioteki Qt5.
Wówczas należy zainstalowć
 - biblioteki Qt5
 - pakietu QGLViewer-qt5 (pakiety: libqglviewer2-qt5, libqglviewer-dev-qt5,
                          libqglviewer-headers)
   ```sh
   sudo apt install libqglviewer2-qt5
   ```
   ```sh
   sudo apt install libqglviewer-dev-qt5
   ```
   ```sh
   sudo apt install libqglviewer-headers
   ```

#W przypadku korzystania z biblioteki Qt6 należy w pliku Makefile
odkomentować dwie pierwsze linie. Ponadto należy też mieć zainstalowane
biblioteki:
 - biblioteki Qt6
 - pakietu QGLViewer-qt6 (pakiety: libqglviewer2-qt6, libqglviewer-dev-qt6,
                          libqglviewer-headers)
   ```sh
   sudo apt install libqglviewer-headers
   ```


#Nazwy i wersje pakietów mogą się różnić w zależności od dystrybucji
Linuksa. Niezmienne zazwyczaj pozostają nazwy typu: libqglviewer-dev-qt5
i libsoil-dev.
Niestety werjsa libqglviewer-qt6 nie jest w pakietach dystrybucyjnych.
Wymaga ona pobrania źródeł z:
```sh
git clone https://github.com/GillesDebunne/libQGLViewer
```
samodzielnej kompilacji i instalacji.

#Chcąc zmienić tło i podać inny plik, należy zmodyfikować
odpowiednio zawartość pliku inc/gsv-BackgroundImage.h
Znajduje się w nim definicja symbolu FILE_BACKGROUND_IMAGE
W miejsce starej nazwy pliku, należy wpisać nazwę własnego pliku
ze ścieżką dostępu (o ile plik nie jest w katalogu bieżącym).

#Numer portu komunikacyjnego znajduje się w pliku: gsv-Const.h

Autor: 
dr inż. Bogdan Kreczmer
