# Contributor: Michael P <ptchinster@archlinux.us>
# Contributor: Roberto Alsina <ralsina@kde.org>
# Contributor: Will Chappell <mr.chapendi@gmail.com>
# Contributor: Jesse Young <jesse.young@gmail.com>
# Contributor: Gustavo Alvarez <sl1pkn07@gmail.com>

pkgname=ragel
pkgver=6.7
pkgrel=1
pkgdesc="Compiles finite state machines from regular languages into executable C, C++, Objective-C, or D code."
arch=('i686' 'x86_64')
url="http://www.complang.org/ragel/"
license=('GPL')
source=("http://www.complang.org/$pkgname/$pkgname-$pkgver.tar.gz")
md5sums=('f4423e0d8a6538dd4e61498fcfad3cec')

build() {
  cd "$srcdir/$pkgname-$pkgver"

  ./configure --prefix=/usr
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"

  make DESTDIR="$pkgdir/" install
}

