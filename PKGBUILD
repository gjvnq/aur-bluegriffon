# Maintainer: liberodark

pkgname=bluegriffon
pkgver=3.1
pkgrel=1
pkgdesc="Responsive Design editor of all Wysiwyg editors"
arch=('x86_64')
url="http://bluegriffon.org/"
license=('GPL')
depends=('xdg-utils')
source_x86_64=("http://bluegriffon.org/freshmeat/${pkgver}/bluegriffon-${pkgver}.Ubuntu18.04-x86_64.deb")
source=($pkgname.desktop
        $pkgname.png)
sha512sums=('ddb86fa39dace6b0f791293ae00bd6d738c82537ddefe089e7812641db5c8362161653e5e7c72aac8955078a2b4ee9319377aa656b27da0b6d737856e641dbba'
         '68f0ae4ce9566d7dbdda49c6c6572d888f121a5d89de3ce0d567f62f9e1062df4e72e9bf1b0fbe67dec7c583abd40dd706817e49653a28c09096bbb33b5bd207')
sha512sums_x86_64=('562753bcfbfcb17ccbc5af7687772fb74fd4a007c5c4317ef2c07a184937b762560ecf47f77a8ee6ea5457e1bed2be6853781cb31b9906a9f6bb23f2a067234f')
        
package() {
  cd $srcdir
  tar xvf data.tar.gz
  cp -r usr $pkgdir
  cp -r opt $pkgdir
  install -vDm644 $srcdir/$pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
  install -vDm644 $srcdir/$pkgname.png $pkgdir/usr/share/pixmaps/$pkgname.png
}
