# Maintainer: liberodark

pkgname=bluegriffon
pkgver=3.0.1
pkgrel=1
pkgdesc="Responsive Design editor of all Wysiwyg editors"
arch=('x86_64')
url="http://bluegriffon.org/"
license=('GPL')
depends=('xdg-utils')
source_x86_64=("http://bluegriffon.org/freshmeat/3.0.1/bluegriffon-3.0.1.Ubuntu16.04-x86_64.deb")
source=($pkgname.desktop
        $pkgname.png)
sha512sums=('ddb86fa39dace6b0f791293ae00bd6d738c82537ddefe089e7812641db5c8362161653e5e7c72aac8955078a2b4ee9319377aa656b27da0b6d737856e641dbba'
         '68f0ae4ce9566d7dbdda49c6c6572d888f121a5d89de3ce0d567f62f9e1062df4e72e9bf1b0fbe67dec7c583abd40dd706817e49653a28c09096bbb33b5bd207')
sha512sums_x86_64=('813f23faf14c612be5cdb54beb6c6517684e90835719c89e58dbed7dc5f49001c04d17db9775da5a67e0ee9a9dfca0fad6dbbf34180d8bf7189ff5a0cc9af9f6')
        
package() {
  cd $srcdir
  tar xvf data.tar.gz
  cp -r usr $pkgdir
  cp -r opt $pkgdir
  install -vDm644 $srcdir/$pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
  install -vDm644 $srcdir/$pkgname.png $pkgdir/usr/share/pixmaps/$pkgname.png
}
