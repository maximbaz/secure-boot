# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Your Name <youremail@domain.com>
pkgname=secure-boot
pkgver=1.0
pkgrel=1
epoch=
pkgdesc="secure-boot tool"
arch=(any)
url=""
license=('GPL')
groups=()
depends=('sbsigntools' 'make' 'efibootmgr')
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(Makefile secure-boot.hook)
noextract=()

package() {
    cd "${srcdir}"
    install -dm700 ${pkgdir}/etc/secure-boot
    install -Dm755 Makefile ${pkgdir}/usr/bin/secure-boot
    install -Dm644 secure-boot.hook ${pkgdir}/etc/pacman.d/hooks/secure-boot.hook
}

md5sums=('385e96af8992f69f3d3065934b3c8dfe'
         '1313074db7ddeac0c115e44c7b16f218')
