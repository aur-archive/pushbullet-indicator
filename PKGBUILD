# Maintainer: agnotek <agnostic[dot]sn[at]gmail[dot]com>

pkgname=pushbullet-indicator
pkgver=0.6.0
_anotherpkgver=14.04.1
_alienpkgrel=0
pkgrel=3
pkgdesc="An indicator for working with PushBullet"
arch=('any')
license=('GPL3')
url="http://www.atareao.es"
options=()
conflicts=()
depends=('python-dbus' 'python-requests' 'python-gobject' 'python-pillow' 'python-ws4py' 'pushbullet-commons' 'libappindicator-gtk3')
optdepends=()
source=("https://launchpad.net/~atareao/+archive/ubuntu/atareao/+files/${pkgname}_${pkgver}-${_alienpkgrel}extras${_anotherpkgver}_all.deb")
md5sums=('4ea9547cbaf815ae27f0fa675bb528b0')

package() {
  cd "${srcdir}"

  ar x "${pkgname}_${pkgver}-${_alienpkgrel}extras${_anotherpkgver}_all.deb" > /dev/null
  tar -xJf data.tar.xz -C "${pkgdir}"
 
  install -d -m755 "${pkgdir}/usr/"
  install -d -m755 "${pkgdir}/opt/"

}

