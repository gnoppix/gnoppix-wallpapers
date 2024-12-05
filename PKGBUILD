# Maintainer: Andreas Mueller <amu@gnoppix.com>  

pkgname=gnoppix-wallpapers
pkgdesc='Wallpapers for Gnoppix'
pkgver=r10.fb98756
pkgrel=1
arch=('any')
url="https://github.com/gnoppix/$pkgname"
license=(GPL-1.0-only)
makedepends=('git')
source=("git+$url.git")
sha512sums=('SKIP')

pkgver() {
   cd $srcdir/$pkgname
   printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
    install -d $pkgdir/usr
    cp -rf $srcdir/$pkgname/usr $pkgdir
}
