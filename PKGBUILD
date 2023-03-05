# Maintainer: Pawel Bogut <pbogut@pbogut.me>

pkgname=qutebrowser-pac-proxy-patch
pkgver=0.1
pkgrel=1
epoch=1
pkgdesc="Patch qutebrowser so that it allows for PAC proxy via chrome proxy-pac-url setting"
arch=('any')
url="https://github.com/pbogut/i3-lock-session"
license=('MIT')
depends=('qutebrowser')
optdepends=()
source=(qutebrowser.hook
        qutebrowser_pac_proxy.patch)
sha512sums=('1ef9896adfc5dab16174c4173eb5ff13459070793e191b6606e399ce4ac47aaa783c45040afbf1880e5c60a15cc7f45a4e9329d56cfa69a62c1c927113df4827'
            '0939fe4fb3966ca5dccbdc3523754e3c391604e1d8e3d0c1b272fc2d89da2c9dfeb0388f29509960860282ac3882bb5d2239ed40af9f1b225297c2c2bb24fd65')


package() {
  install -m0644 -D qutebrowser.hook "$pkgdir"/etc/pacman.d/hooks/qutebrowser-pac-proxy.hook
  install -m0644 -D qutebrowser_pac_proxy.patch "$pkgdir"/usr/share/qutebrowser-pac-proxy-patch/proxy.patch
}
