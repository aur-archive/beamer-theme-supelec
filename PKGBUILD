# Maintainer: Thibault Suzanne <thi [DOT] suzanne [AT] gmail [DOT] com>
pkgname=beamer-theme-supelec  
pkgver=1.0
pkgrel=3
pkgdesc="Supelec theme for beamer"
url="http://wwwdi.supelec.fr/fb/download/LaTeX/beamersupelec/tex/latex/splcbeam/"
arch=("any")
license=("unknown")
depends=("texlive-core")
makedepends=("unzip")
source=("http://wwwdi.supelec.fr/fb/download/LaTeX/beamersupelec/splcbeam-1.0.zip")
md5sums=('3227bde86fa27803ac0e22cb5d929900')

build() {
  mkdir -p ${pkgdir}/usr/share/texmf-dist/tex/latex/beamer/themes/{color,font,inner,outer,theme} 
  mkdir -p ${pkgdir}/usr/share/texmf-dist/tex/latex/beamer/art/images

  cd "$srcdir/beamersupelec/tex/latex/splcbeam"
  install -m644 beamercolorthemesupelec.sty $pkgdir/usr/share/texmf-dist/tex/latex/beamer/themes/color/
  install -m644 beamerfontthemesupelec.sty $pkgdir/usr/share/texmf-dist/tex/latex/beamer/themes/font/
  install -m644 beamerinnerthemesupelec.sty $pkgdir/usr/share/texmf-dist/tex/latex/beamer/themes/inner/
  install -m644 beamerouterthemesupelec.sty $pkgdir/usr/share/texmf-dist/tex/latex/beamer/themes/outer/
  install -m644 beamerthemesupelec.sty $pkgdir/usr/share/texmf-dist/tex/latex/beamer/themes/theme/
  install -m644 beamerthemesupeleclogo.pdf $pkgdir/usr/share/texmf-dist/tex/latex/beamer/art/images/
  install -m644 beamerthemesupeleclogo.eps $pkgdir/usr/share/texmf-dist/tex/latex/beamer/art/images/
}
