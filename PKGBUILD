# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Eoghan West <eowest@gmail.com>
pkgname=vital-synth-desktop-file-git
pkgver=0.0.1
pkgrel=1
epoch=
pkgdesc="a deskotp file for the Vital eavetable synth software"
arch=()
url="https://github.com/calacuda/vital-desktop-aur"
license=('MIT')
groups=()
depends=(vital-synth)
makedepends=()
checkdepends=()
optdepends=()
provides=(vital-synth-desktop-file)
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("$pkgname-$pkgver.tar.gz"
        "$pkgname-$pkgver.patch")
noextract=()
sha256sums=()
validpgpkeys=()

prepare() {
	cd "$pkgname-$pkgver"
	# patch -p1 -i "$srcdir/$pkgname-$pkgver.patch"
}

build() {
	cd "$pkgname-$pkgver"
	# ./configure --prefix=/usr
	# make
}

package() {
	cd "$pkgname-$pkgver"
	# make DESTDIR="$pkgdir/" install
	install ./vital-synth.desktop /usr/share/applications/vital-synth.desktop
	install ./vital.png /usr/share/pixmaps/vital.png
}
