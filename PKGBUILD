
#
# Maintainer: Paul Dunn <pwjdunn AT gmail DOT com>
#

pkgname=xpsfan_smm
pkgver=0.1
pkgrel=1
arch=('i686' 'x86_64')
license=('')
depends=('intel-gpu-tools')
makedepends=('gcc-multilib')
options=('!strip')
source=("https://launchpad.net/i8kutils/trunk/1.42/+download/i8kutils_1.42.tar.xz")

sha256sums=('SKIP')
validpgpkeys=()

build() {
        gcc -m32 -o "$srcdir/"smm "$srcdir"/i8kutils/smm.c
}

package() {
        install -Dm755 "$srcdir"/smm "$pkgdir"/usr/local/bin/smm
        install -Dm755 "$srcdir"/../xps_fan-lock "$pkgdir"/usr/local/bin/xps_fan-lock
        install -Dm755 "$srcdir"/../xps_fan-unlock "$pkgdir"/usr/local/bin/xps_fan-unlock
	install -Dm755 "$srcdir"/../xps_original "$pkgdir"/usr/local/bin/xps_original
	install -Dm755 "$srcdir"/../xps_silent "$pkgdir"/usr/local/bin/xps_silent
	chmod +x "$pkgdir"/usr/local/bin/smm
	chmod +x "$pkgdir"/usr/local/bin/xps_fan-lock
	chmod +x "$pkgdir"/usr/local/bin/xps_fan-unlock
        chmod +x "$pkgdir"/usr/local/bin/xps_fan-original
        chmod +x "$pkgdir"/usr/local/bin/xps_fan-silent
}

