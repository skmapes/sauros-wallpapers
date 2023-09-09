# Maintainer: Sean Makes <skmapes@liberty.edu>

pkgname=sauros-wallpapers
pkgver=1.0
pkgrel=5
pkgdesc="Default wallpapers for saurOS"
url="https://github.com/skmapes/sauros-wallpapers"
arch=('any')
license=('GPL3')
makedepends=()
depends=()
conflicts=()
groups=(sauros-wallpapers)
provides=("${pkgname}")
options=(!strip !emptydirs)

prepare() {
	cp -af ../files/. ${srcdir}
}

package() {
	local _bgdir=${pkgdir}/usr/share/backgrounds
	mkdir -p "$_bgdir"
	cp -r ${srcdir}/* "$_bgdir"
}