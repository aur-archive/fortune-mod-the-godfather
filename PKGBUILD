# Maintainer: Jeff Sharpe <jeff@impcode.com>
# Contributor: Rick W. Chen <stuffcorpse at archlinux dot us>

pkgname=fortune-mod-the-godfather
pkgver=3.0
pkgrel=3
pkgdesc="The Godfather fortune cookie files"
arch=('any')
url="https://github.com/jetm/fortune-epigrams"
makedepends=('fortune-mod')
groups=('fortune-mods')
license=(none)
source=("https://raw.github.com/jetm/fortune-epigrams/master/the-godfather")
md5sums=('446d4d6be61e3fd06c4c3b98eb590c49')

build()
{
	strfile "${srcdir}/the-godfather" "${srcdir}/the-godfather.dat"
}

package() {
	install -D -m644 "${srcdir}/the-godfather" \
		"${pkgdir}/usr/share/fortune/the-godfather"
	install -D -m644 "${srcdir}/the-godfather.dat" \
		"${pkgdir}/usr/share/fortune/the-godfather.dat"
}
