# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-sale-shipment-grouping
_pkgname=trytond_sale_shipment_grouping
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The sale_shipment_grouping module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-party>=3.4' 'trytond-stock>=3.4' 'trytond-sale>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("dbe3b253e8019d46a471ae108b14124c")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}