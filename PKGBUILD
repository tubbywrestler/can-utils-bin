# Maintainer: piratecarrot

pkgname=can-utils-bin
pkgver=2025.01
_pkgrel_src=3
pkgrel=1
pkgdesc="Linux-CAN / SocketCAN user space applications (precompiled)"
arch=('x86_64')
url="https://github.com/linux-can/can-utils"
license=('GPL-2.0-only')
provides=('can-utils')
conflicts=('can-utils' 'can-utils-git')

source=("https://github.com/tubbywrestler/can-utils-bin/releases/download/${pkgver}-${_pkgrel_src}/can-utils-${pkgver}-${_pkgrel_src}-x86_64.pkg.tar.zst")
sha256sums=('1b18a0f421076a880f49aacbcdaf169e9d3490b979824320eb001295712be683')

package() {
    bsdtar -xf "${srcdir}/can-utils-${pkgver}-${_pkgrel_src}-x86_64.pkg.tar.zst" -C "${pkgdir}" --exclude .PKGINFO --exclude .BUILDINFO --exclude .MTREE
}
