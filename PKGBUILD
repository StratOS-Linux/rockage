pkgname=rock
pkgver=1.0
pkgrel=0
pkgdesc="Package manager wrapper for StratOS"
arch=("any")
url="https://github.com/StratOS-Linux/rock"
license=('GPL')
depends=('bash')
optdepends=('yay-bin: AUR support'
	    'flatpak: Flatpak support'
	    'snapd: snap support'
	    )
source=("git+https://github.com/StratOS-Linux/${pkgname}.git")
sha1sums=('SKIP')

package() {
    cd "$pkgname"
    mkdir -p $pkgdir/usr/bin
    install -D -m755 ./rock $pkgdir/usr/bin/$pkgname
}
