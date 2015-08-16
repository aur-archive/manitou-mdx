# Maintainer: Mladen Pejakovic <pejakm@gmail.com>

pkgname=manitou-mdx
pkgver=1.3.0
pkgdesc="Database-driven email system: mail-database exchanger"
pkgrel=2
arch=(i686 x86_64)
url="http://www.manitou-mail.org/"
license=(GPL)
makedepends=()
depends=('qt4' 'perl' 'perl-dbi' 'perl-dbd-pg' 'perl-bit-vector' 'perl-digest-sha1' 'perl-mime-tools')
options=()
source=(http://www.manitou-mail.org/source/${pkgname}-${pkgver}.tar.gz)
md5sums=('d1c67d4498c623b15285a701cbae70a6')

build(){
  cd ${srcdir}/${pkgname}-${pkgver}
  perl Makefile.PL
  make
}

package(){
  cd ${srcdir}/${pkgname}-${pkgver}
  make DESTDIR="${pkgdir}" install
}
