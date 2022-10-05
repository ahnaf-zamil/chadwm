# Maintainer: DevGuyAhnaf <ahnaf@ahnafzamil.com>
pkgname=chadwm-devguyahnaf
_pkgname=chadwm
_output_dir=~/.config/chadwm
pkgver=0.0.1
pkgrel=1
epoch=1
pkgdesc="DevGuyAhnaf's version of ChadWM (DWM Modif)"
arch=('x86_64' 'i686')
url="https://github.com/ahnaf-zamil/chadwm"
license=('MIT')
groups=()
depends=('picom' 'feh' 'acpi' 'rofi' 'pavucontrol' 'dash' 'imlib2' 'xorg-xsetroot' 'wget' 'xorg-server')
makedepends=()
checkdepends=()
optdepends=()
provides=('dwm')
conflicts=('dwm')
source=("$_pkgname::git+https://github.com/ahnaf-zamil/chadwm.git")
sha256sums=('SKIP')

build() {
	cd "$_pkgname"
	mkdir "$_output_dir"
	cp -r "./" "$_output_dir"
}

package() {
	cd "$_output_dir/chadwm"
	sudo make clean install
}
