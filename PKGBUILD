pkgname=pdf2png
pkgver=1.0
pkgrel=1
pkgdesc="PDF to PNG converter using PyMuPDF"
arch=('any')
url="https://github.com/xingzhou1002/pdf2png"
license=('EPL')
depends=('python-pymupdf')
source=("pdf2png.py")
sha256sums=('SKIP')

package() {
  install -Dm755 "$srcdir/pdf2png.py" "$pkgdir/usr/bin/pdf2png"
}