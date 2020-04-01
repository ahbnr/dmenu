pkgname=dmenu-custom
pkgver=r1097.70f3fec
pkgrel=1
pkgdesc="Generic menu for X. With borders and centering patch."
arch=('x86_64')
url="https://tools.suckless.org/dmenu/"
license=('MIT')
provides=('dmenu')
depends=('sh' 'libxinerama' 'libxft' 'freetype2')

prepare() {
  cp -R $startdir/* $srcdir || true
}

build() {
  ./build.sh
}

package() {
  make PREFIX=/usr DESTDIR="$pkgdir" install
  install -m644 -D LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
