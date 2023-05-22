pkgname=cdwin
pkgver=r17.ab8e7d3
pkgrel=1
pkgdesc="CD to a Windows-formatted path in any WSL terminal"
arch=("any")
url="https://github.com/justalemon/cdwin"
license=("MIT")
depends=("bash")
makedepends=()
provides=("${pkgname%-git}")
source=("src-$pkgname::git+${url}.git")
sha256sums=('SKIP')

pkgver() {
    cd "src-$pkgname"
    printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short=7 HEAD)"
}

package() {
    cd "src-$pkgname"
    install -m 644 -DT "$startdir/$pkgname.sh" "$pkgdir/etc/profile.d/$pkgname.sh"
}

post_install() {
    # shellcheck source=cdwin.sh
    source "$pkgdir/etc/profile.d/$pkgname.sh"
    echo -e "\033[1;33mWarning! \033[1;37mcdwin will only work on posix compliant terminals"
}
