# Contributor: Andrea Scarpino <bash.lnx@gmail.com>
# Contributor: Volker Lorrmann <lorrmann@physik.uni-wuerzburg.de>

pkgname=octplot
pkgver=0.4.0
pkgrel=1
pkgdesc="A handle graphics package for Octave, the free alternative to matlab."
arch=('i686' 'x86_64')
url="http://octplot.sourceforge.net/"
license=('GPL')
depends=('octaveforge>=2006.03.17' 'fltk' 'freetype1' 'ghostscript')
source=(http://downloads.sourceforge.net/$pkgname/$pkgname-$pkgver.tar.gz)
md5sums=('1ea6fa85b620e6af252ee64407c87285')

build() {
  cd $startdir/src/$pkgname-$pkgver
  ./configure --prefix=/usr
  make || return 1
  make DESTDIR=$startdir/pkg install
}
