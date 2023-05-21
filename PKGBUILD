pkgname=cdwin
pkgver=0.0.1
pkgrel=1
pkgdesc="CD to a Windows-formatted path in any WSL terminal"
arch=("any")
url="https://github.com/justalemon/cdwin"
license=("MIT")
depends=("bash")

package() {
    install -m 644 -DT "$startdir/$pkgname.sh" "$pkgdir/etc/profile.d/$pkgname.sh"
}

post_install() {
    # shellcheck source=cdwin.sh
    source "$pkgdir/etc/profile.d/$pkgname.sh"
    echo -e "\033[1;33mWarning! \033[1;37mcdwin will only work on posix compliant terminals"
}
