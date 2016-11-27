
#
# Maintainer: Paul Dunn <pwjdunn AT gmail DOT com>
#

pkgname=xpsfan_smm
pkgver=0.1
pkgrel=1
arch=('i686' 'x86_64')
license=('')
depends=('')
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
        install -Dm755 "$srcdir"/../fan_off "$pkgdir"/usr/local/bin/fan_off
        install -Dm755 "$srcdir"/../fan_on "$pkgdir"/usr/local/bin/fan_on
	chmod +x "$pkgdir"/usr/local/bin/smm
	chmod +x "$pkgdir"/usr/local/bin/fan_off
	chmod +x "$pkgdir"/usr/local/bin/fan_on
}

