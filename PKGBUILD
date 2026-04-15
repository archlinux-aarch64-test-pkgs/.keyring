pkgname=aarch64-addons-keyring
pkgver=20260415
pkgrel=1
pkgdesc='Keyring for the aarch64-addons repository'
arch=('any')
url='https://github.com/archlinux-aarch64-test-pkgs'
license=('GPL-3.0-or-later')
install="${pkgname}.install"
source=('aarch64-addons.gpg'
        'aarch64-addons-trusted'
        'aarch64-addons-revoked')
sha256sums=('SKIP'
            'SKIP'
            'SKIP')

package() {
    install -Dm644 aarch64-addons.gpg \
        "${pkgdir}/usr/share/pacman/keyrings/aarch64-addons.gpg"
    install -Dm644 aarch64-addons-trusted \
        "${pkgdir}/usr/share/pacman/keyrings/aarch64-addons-trusted"
    install -Dm644 aarch64-addons-revoked \
        "${pkgdir}/usr/share/pacman/keyrings/aarch64-addons-revoked"
}
