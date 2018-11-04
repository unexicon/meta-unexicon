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
    'meta-unexicon-ides')
pkgbase='meta-unexicon'
pkgver=1.7
pkgrel=1
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
         `cat packages-ides.lst|sed -r 's,[[:space:]]*#.*,,'`)
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
        packages-ides.lst)

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
  pkgdesc="Packages that were to big for the live system"
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

md5sums=('ce02d3c73f7c87a29ebda2c7d55ac151'
         '6920b66c7332743d1f61efd9df93245d'
         '71ed5b2d204e211fb821baf9f7fced82'
         'cd9b1e648fac9f060f238755fb77a920'
         'f9c34b351dde4bb01c9e1d8258e50d95'
         'e346bec5cb4c50e7814ac566a1dc1244'
         'a4ae67d8e911bb85f69a9c5c4ab9ee1e'
         'cecd4131d2129a2555f26e941b21be17'
         'b17a8d069ecc206adcfc56f38e6f72c7'
         '70252603bb04f226e4d10821926bb1ab'
         '6232764eecad85dc706274dbf982386d'
         '828b607f5a5a7713b00a61214ff74906'
         'f28c680e28ab0ece1702d5b9a736b137'
         '4e647cf9c0a4dfda7b9c6a95a159e898'
         'd1d8a7fe93a98cc0c9ff187a67e07847'
         'd000feb334312565b285a40b2ae17a8c')
