# Maintainer: Damjan Georgievski <gdamjan@gmail.com>
pkgname=secure-boot
pkgver=1.2
pkgrel=1
epoch=
pkgdesc="secure-boot tool"
arch=(any)
url="https://github.com/gdamjan/secure-boot"
license=('GPL')
groups=()
depends=('efitools' 'sbsigntools' 'make' 'efibootmgr' 'util-linux' 'binutils' 'systemd')
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
source=("secure-boot" "secure-boot.hook" "95-secure-boot.install")
noextract=()

package() {
    cd "${srcdir}"
    install -dm700 "${pkgdir}"/etc/secure-boot
    install -Dm755 secure-boot "${pkgdir}"/usr/bin/secure-boot
    install -Dm644 secure-boot.hook "${pkgdir}"/usr/share/libalpm/hooks/99-secure-boot.hook
    install -Dm644 95-secure-boot.install "${pkgdir}"/usr/lib/kernel/install.d/
}

md5sums=('0f737d39fd67020dbecf1cd6ad63b9b8'
         '1313074db7ddeac0c115e44c7b16f218'
         '31dd53c29726a92f498b4b56d9684032')
