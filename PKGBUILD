# Maintainer: archcrack <johndoe.arch@outlook.com>

pkgname=pacrep
pkgver=0.1.3
pkgrel=1
pkgdesc="Choose pacman repositories on a per package basis"
arch=(any)
url="https://github.com/leo-arch/pacrep"
license=(GPL2)
depends=('bash' 'pacman' 'coreutils' 'grep' 'gawk')
makedepends=('git')
source=("git+${url}.git")
sha256sums=('SKIP')

package() {
  cd "${srcdir}/${pkgname}"
  install -Dm755 $pkgname "${pkgdir}/usr/bin/$pkgname"
}
