# Maintainer: Panda <panda@fydeos.io>

pkgname=fyde-mirrorlist
filename=fyde-mirrorlist
pkgver=20240823
pkgrel=1
pkgdesc="Mirrorlist for Fyde Arch linux images"
arch=('any')
url=""
license=('GPL3')
source=(${filename})
install=${pkgname}.install
sha256sums=('9ee39aeef292507bcbe6b6b703eeb71626af3e378e8e65f82a2b8e9a35aca02f')

pkgver() {
    date +%Y%m%d
}

package() {
  mkdir -p ${pkgdir}/etc/pacman.d
  install -m644 ${srcdir}/${filename} ${pkgdir}/etc/pacman.d/${filename}-new
}
