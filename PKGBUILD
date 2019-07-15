pkgname=amdgpu-overclock
pkgver=0.1
pkgrel=1
arch=('any')
license=('GPL2')
depends=('systemd')

source=('amdgpu-overclock' 'amdgpu-overclock.service' 'amdgpu-overclock.cfg')
sha256sums=('c099373116b90b0ace10ba7688c8cd36e5ed251a5a3e3ef451f946f53ec99b79'
            'df5abfb22e53d24b9bfd196e4c31276c2e0f0bc9dca94890783d776abeb2cd2b'
            '3a9ef714711db755dc2b80487a4424b4ecb46cebbd89ee2ca8269daa644c69e7')

package() {
    mkdir -p ${pkgdir}/usr/bin
    cp ${srcdir}/amdgpu-overclock ${pkgdir}/usr/bin/
    mkdir -p ${pkgdir}/usr/lib/systemd/system
    cp ${srcdir}/amdgpu-overclock.service ${pkgdir}/usr/lib/systemd/system/
    mkdir -p ${pkgdir}/etc
    cp ${srcdir}/amdgpu-overclock.cfg ${pkgdir}/etc/
}
