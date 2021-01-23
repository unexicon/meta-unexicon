# vim:set ts=2 sw=2 et:
# Maintainer: Brian Bidulock <bidulock@openss7.org>
pkgname=(
    'meta-unexicon'
    'meta-unexicon-inst'
    'meta-unexicon-live'
    'meta-unexicon-plus'
    'meta-unexicon-arch'
    'meta-unexicon-xtra'
    'meta-unexicon-xvid'
    'meta-unexicon-desk'
    'meta-unexicon-kids'
    'meta-unexicon-elec'
    'meta-unexicon-draw'
    'meta-unexicon-devl'
    'meta-unexicon-geog'
    'meta-unexicon-virt'
    'meta-unexicon-more'
    'meta-unexicon-note'
    'meta-unexicon-most'
    'meta-unexicon-ides'
    'meta-unexicon-dcam'
    'meta-unexicon-adev'
    'meta-unexicon-clus'
    'meta-unexicon-data')
pkgbase='meta-unexicon'
pkgver=1.10
pkgrel=6
pkgdesc="A collection of meta packages for the unexicon distribution"
arch=('any')
url="http://www.unexicon.com"
license=('GPL')
groups=('unexicon')
depends=(`cat packages-inst.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-live.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-plus.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-arch.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-xtra.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-xvid.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-desk.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-kids.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-elec.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-draw.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-devl.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-geog.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-virt.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-more.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-note.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-ides.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-dcam.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-adev.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-clus.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-data.lst|sed -r 's,[[:space:]]*#.*,,'`)
depends=()
source=(packages-inst.lst
        packages-live.lst
        packages-plus.lst
        packages-arch.lst
        packages-xtra.lst
        packages-xvid.lst
        packages-desk.lst
        packages-kids.lst
        packages-elec.lst
        packages-draw.lst
        packages-devl.lst
        packages-geog.lst
        packages-virt.lst
        packages-more.lst
        packages-note.lst
        packages-ides.lst
        packages-dcam.lst
        packages-adev.lst
        packages-clus.lst
        packages-data.lst)

package_meta-unexicon() {
  pkgdesc="A meta package for unexicon (remove me)"
  depends=()
  install -Dm644 <(echo "") "$pkgdir/usr/share/unexicon/installed/meta-unexicon"
}

package_meta-unexicon-inst() {
  pkgdesc="The unexicon install system"
  depends=('meta-unexicon' 'meta-unexicon-arch' `cat packages-inst.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-inst.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-inst"
}

package_meta-unexicon-live() {
  pkgdesc="The unexicon live system"
  depends=('meta-unexicon' `cat packages-live.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-live.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-live"
}

package_meta-unexicon-plus() {
  pkgdesc="Extra packages for the unexicon live system"
  depends=('meta-unexicon' 'meta-unexicon-live' `cat packages-plus.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-plus.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-plus"
}

package_meta-unexicon-arch() {
  pkgdesc="Packages included on the Arch Linux install disk"
  depends=('meta-unexicon' `cat packages-arch.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-arch.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-arch"
}

package_meta-unexicon-xtra() {
  pkgdesc="Packages that were too big for the live system"
  depends=('meta-unexicon' `cat packages-xtra.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-xtra.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-xtra"
}

package_meta-unexicon-xvid() {
  pkgdesc="Packages that supports OpenGL video and more video cards"
  depends=('meta-unexicon' `cat packages-xvid.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-xvid.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-xvid"
}

package_meta-unexicon-desk() {
  pkgdesc="Packages for a full blown desktop"
  depends=('meta-unexicon' `cat packages-desk.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-desk.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-desk"
}

package_meta-unexicon-kids() {
  pkgdesc="Packages for the kids"
  depends=('meta-unexicon' `cat packages-kids.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-kids.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-kids"
}

package_meta-unexicon-elec() {
  pkgdesc="Packages for electronics design"
  depends=('meta-unexicon' `cat packages-elec.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-elec.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-elec"
}

package_meta-unexicon-draw() {
  pkgdesc="Packages for digital drawing and painting"
  depends=('meta-unexicon' `cat packages-draw.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-draw.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-draw"
}

package_meta-unexicon-devl() {
  pkgdesc="Packages for software development"
  depends=('meta-unexicon' `cat packages-devl.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-devl.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-devl"
}

package_meta-unexicon-geog() {
  pkgdesc="Packages for containing large geographic data"
  depends=('meta-unexicon' `cat packages-geog.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-geog.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-geog"
}

package_meta-unexicon-virt() {
  pkgdesc="Packages for virtualization"
  depends=('meta-unexicon' `cat packages-virt.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-virt.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-virt"
}

package_meta-unexicon-more() {
  pkgdesc="More unexicon packages yet: candidates to be included"
  depends=('meta-unexicon' `cat packages-more.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-more.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-more"
}

package_meta-unexicon-note() {
  pkgdesc="Packages primarily suitable for notebook computers."
  depends=('meta-unexicon' `cat packages-note.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-note.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-note"
}

package_meta-unexicon-most() {
  pkgdesc="All unexicon meta packages"
  depends=('meta-unexicon' 'meta-unexicon-live' 'meta-unexicon-plus' 'meta-unexicon-arch' 'meta-unexicon-xtra' 'meta-unexicon-xvid' 'meta-unexicon-desk' 'meta-unexicon-elec' 'meta-unexicon-devl' 'meta-unexicon-geog' 'meta-unexicon-virt' 'meta-unexicon-more' 'meta-unexicon-kids' 'meta-unexicon-draw')
}

package_meta-unexicon-ides() {
  pkgdesc="Packages for Industrial Design."
  depends=('meta-unexicon' `cat packages-ides.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-ides.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-ides"
}

package_meta-unexicon-dcam() {
  pkgdesc="Packages for Digital Cameras."
  depends=('meta-unexicon' `cat packages-dcam.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-dcam.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-dcam"
}

package_meta-unexicon-adev() {
  pkgdesc="Packages for Archlinux Development."
  depends=('meta-unexicon' `cat packages-adev.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-adev.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-adev"
}

package_meta-unexicon-clus() {
  pkgdesc="Packages for Clustering and Cloud Development."
  depends=('meta-unexicon' `cat packages-clus.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-clus.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-clus"
}

package_meta-unexicon-data() {
  pkgdesc="Packages for Data search and visualization."
  depends=('meta-unexicon' `cat packages-data.lst|sed -r 's,[[:space:]]*#.*,,'`)
  install -Dm644 packages-data.lst "$pkgdir/usr/share/unexicon/installed/meta-unexicon-data"
}

md5sums=('d76b5d7192135001bd261fec983c9cdd'
         '0d828f39c582a566e25efaebd24938cc'
         '02b8c01406acf4840ecc8fd603e52d45'
         '8def2fbb05b1bc14e736faddcaa6ecda'
         '665f784d5e06aba38f63feb8eb9d8c3b'
         '25cc2d408b319e9fce6e57faae13b2b3'
         'd035e94050a9b290afff645630589442'
         'e5919073865fc184e9d0fbe57f11d612'
         'b17a8d069ecc206adcfc56f38e6f72c7'
         '1d3264a4752df8703817bee9c5de8d38'
         'f4a6f7bb10d1089ea2c4f4da23b2d99a'
         '828b607f5a5a7713b00a61214ff74906'
         '3f0c382687c73178bcb8ac47ed62f730'
         '6625e6e9c5389767f6e2506f23aed512'
         'd275ada02a4fd3a4479359b85a7c2314'
         'd000feb334312565b285a40b2ae17a8c'
         'b4678c1aacbcd233ad802bcf07e117e2'
         '840337d654dd0cb6d882295bc97b05ae'
         '541860919ee5151ef6576bcfe2846fc5'
         'de0f113ed4011960a949c8923db8f03c')
