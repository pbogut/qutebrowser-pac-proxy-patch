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
sha512sums=('df734dec16b126887c470a2b3c566f3d4256f14bbd2d0435fea0f5c2806b1ccc74b65626dafad1ee21e8adfd6818a7a8b28d2a91b52d5b92986662b945d71e14'
            '0939fe4fb3966ca5dccbdc3523754e3c391604e1d8e3d0c1b272fc2d89da2c9dfeb0388f29509960860282ac3882bb5d2239ed40af9f1b225297c2c2bb24fd65')


package() {
  install -m0644 -D qutebrowser.hook "$pkgdir"/etc/pacman.d/hooks/qutebrowser-pac-proxy.hook
  install -m0644 -D qutebrowser_pac_proxy.patch "$pkgdir"/usr/share/qutebrowser-pac-proxy-patch/proxy.patch
}
