#Maintainer: Simone Sclavi 'Ito' <darkhado@gmail.com>

pkgname=spacephallus
pkgver=1.2
pkgrel=4
arch=('i686' 'x86_64')
__pkgalias=SpacePhallusLinux
pkgdesc="A fun shoot-em-up in which you fight against hordes of evil space penises"
url="http://www.charliesgames.com/wordpress/?page_id=18"
if [ $CARCH = "i686" ]; then
    depends=( 'freetype2' 'libxrandr' 'mesa')
else
    depends=( 'lib32-mesa' 'lib32-libxrandr' 'lib32-freetype2' 'lib32-libxxf86vm')
fi
license=('custom')
source=(http://www.charliesgames.com/phallus/${__pkgalias}.tar.gz
        spacephallus.desktop)

md5sums=('83a8f714d8b61ba63dd24082d52642de'
         'c68d7f08f8560309552654691954f518')
package(){
    install -m644 -D spacephallus.desktop $pkgdir/usr/share/applications/pacephallus.desktop
    cd $__pkgalias
    install -m755 -D Space\ Phallus $pkgdir/usr/bin/SpacePhallus
    install -m644 -D phalluslogo.png $pkgdir/usr/share/pixmaps/phalluslogo.png
}

