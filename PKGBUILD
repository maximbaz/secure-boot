# Maintainer: Damjan Georgievski <gdamjan@gmail.com>
pkgname=secure-boot
pkgver=1.0
pkgrel=1
epoch=
pkgdesc="secure-boot tool"
arch=(any)
url="https://github.com/gdamjan/secure-boot"
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
source=(secure-boot secure-boot.hook)
noextract=()

package() {
    cd "${srcdir}"
    install -dm700 ${pkgdir}/etc/secure-boot
    install -Dm755 secure-boot ${pkgdir}/usr/bin/secure-boot
    install -Dm644 secure-boot.hook ${pkgdir}/etc/pacman.d/hooks/secure-boot.hook
}

md5sums=('8ce6985cddeea10d91bd6b785c9df557'
         '1313074db7ddeac0c115e44c7b16f218')
