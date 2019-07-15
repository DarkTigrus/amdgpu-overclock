pkgname=amdgpu-overclock
pkgver=0.1
pkgrel=1
arch=('any')
license=('GPL2')
depends=('systemd')

source=('amdgpu-overclock' 'amdgpu-overclock.service' 'amdgpu-overclock.cfg')
sha256sums=('56ce5c90cfacf142b2ce3c9650c52a30498b61f5d3080f74874745f089382f06'
            'f7e6e9d0245768705f42f08b587261b75aa9719c014a790b1aec0c57e3673a90'
            '3a9ef714711db755dc2b80487a4424b4ecb46cebbd89ee2ca8269daa644c69e7')

package() {
    mkdir -p ${pkgdir}/usr/bin
    cp ${srcdir}/amdgpu-overclock ${pkgdir}/usr/bin/
    mkdir -p ${pkgdir}/usr/lib/systemd/system
    cp ${srcdir}/amdgpu-overclock.service ${pkgdir}/usr/lib/systemd/system/
    mkdir -p ${pkgdir}/etc
    cp ${srcdir}/amdgpu-overclock.cfg ${pkgdir}/etc/
}
