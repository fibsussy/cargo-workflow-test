pkgname=cargo-workflow-test
pkgver=0.0.0
pkgrel=1
pkgdesc="literally does nothing but print the vesrion"
arch=('x86_64' 'aarch64')
url="https://github.com/fibsussy/$pkgname"
license=('MIT')
depends=()
makedepends=('curl')
source=("https://github.com/fibsussy/$pkgname/releases/download/v${pkgver}/$pkgname-linux-${CARCH}.tar.gz"
        "https://raw.githubusercontent.com/fibsussy/$pkgname/main/LICENSE")
sha256sums=('SKIP'
            'SKIP')
options=('!debug')

package() {
    install -Dm755 "$pkgname" "$pkgdir/usr/bin/$pkgname"
    install -Dm644 "LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
