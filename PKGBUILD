# Maintainer: Erik Dubois <erik.dubois@gmail.com>
pkgname=my-xfce-config
_pkgname=my-xfce-config
pkgver=22.07
pkgrel=01
_destname1="/etc/skel/"
_destname2="/usr/share/themes/"
pkgdesc="Personal config for xfce4"
arch=('any')
url="https://github.com/Khori-Lee/${_pkgname}.git"
license=('GPL3')
makedepends=('git')
provides=("${pkgname}")
conflicts=()
options=(!strip !emptydirs)
source=(${_pkgname}::"git+${url}")
sha256sums=('SKIP')
package() {
	install -dm 755 ${pkgdir}${_destname1}
	install -dm 755 ${pkgdir}${_destname2}
	rm ${srcdir}/${_pkgname}/git*
	rm ${srcdir}/${_pkgname}/setup*
    cp -r ${srcdir}/${_pkgname}/${_destname1}/. ${pkgdir}${_destname1}
}
