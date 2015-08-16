# Maintainer: Sebastien Luttringer <seblu+arch@seblu.net>
# Contributor: Bartek Piotrowski <barthalion@gmail.com>
# Contributor: cromo <dawid@klej.net>

pkgname=laptop-detect
pkgver=0.13.7
pkgrel=2
pkgdesc='Attempts to detect a laptop'
arch=('i686' 'x86_64')
url='http://packages.qa.debian.org/l/laptop-detect.html'
license='BSD' 
depends=('dmidecode') 
source=("http://cdn.debian.net/debian/pool/main/l/${pkgname}/${pkgname}_${pkgver}.tar.gz")
md5sums=('b5b3dab84ca03b66c8501dc8a98f9c91')

package() { 
    cd ${pkgname}
    sed -e "s/@VERSION@/${pkgver}/g" < laptop-detect.in > laptop-detect
    install -D -m755 laptop-detect "$pkgdir/usr/sbin/laptop-detect"
}

# vim:set ts=2 sw=2 ft=sh et:
