pkgname=cdw
pkgver=0.0.1
pkgrel=1
pkgdesc="CD to a Windows-formatted path in any WSL terminal"
arch=("any")
url="https://github.com/justalemon/cdw"
license=("MIT")
depends=("bash")

package() {
    install -m 775 -DT "$startdir/$pkgname.sh" "$pkgdir/usr/bin/$pkgname"
}
