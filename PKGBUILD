# Maintainer: carukia <hornetsnest0@gmail.com
# Contributor: tanuva <tanuva aet nightsoul d00t org>
# Contributor: qwer1234
pkgname='gtk-theme-adwaita-cupertino'
pkgver=2.1.5
pkgrel=2
pkgdesc="Adwaita Cupertino GTK3 theme with matte metacity icons"
arch=(any)
url="http://gnome-look.org/content/show.php?content=147061"
license=('GPL')
depends=('gtk-engine-unico' 'gtk-engine-murrine')
conflicts=('gtk-theme-adwaita-cupertino-glassy')
source=('http://gnome-look.org/CONTENT/content-files/147061-Adwaita-Cupertino.tar.gz')
md5sums=('982e7ce13fe39eaf548ca484a79a1e5f')
install=gtk-theme-adwaita-cupertino.install

package() {
 	bsdtar -xf ${srcdir}/147061-Adwaita-Cupertino.tar.gz
	mkdir -p ${pkgdir}/usr/share/themes
	cp -R ${srcdir}/Adwaita*  ${pkgdir}/usr/share/themes/
	cd ${pkgdir}/usr/share/themes/
	find . -type f -exec chmod 644 {} \;
	find . -type d -exec chmod 755 {} \;
}
