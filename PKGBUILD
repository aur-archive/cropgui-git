pkgname=cropgui-git
arch=('any')
pkgver=20150315
pkgrel=1
pkgdesc="A simple tool for lossless jpeg cropping"
license=('GPL')
url="http://emergent.unpythonic.net/01248401946"
depends=('pygtk' 'python2-imaging' 'jpegexiforient')
provides=('cropgui')
conflicts=('cropgui')
source=('cropgui-git::git+https://github.com/jepler/cropgui.git')
md5sums=('SKIP')

prepare() {
cd $pkgname
sed -i '1s/python/python2/' *.py
}

package() {
cd $pkgname
./install.sh -P /usr/bin/python2 -p /usr -t $pkgdir
}
