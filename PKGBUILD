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
    'meta-unexicon-devl'
    'meta-unexicon-geog'
    'meta-unexicon-virt'
    'meta-unexicon-more'
    'meta-unexicon-most')
pkgbase='meta-unexicon'
pkgver=1.4
pkgrel=25
pkgdesc="A collection of meta packages for the unexicon distribution"
arch=('any')
url="http://www.unexicon.com"
license=('GPL')
groups=('unexicon')
depends=()
depends=(`cat packages-inst.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-live.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-plus.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-arch.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-xtra.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-xvid.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-desk.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-kids.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-elec.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-devl.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-geog.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-virt.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-more.lst|sed -r 's,[[:space:]]*#.*,,'`)
source=(packages-inst.lst
        packages-live.lst
        packages-plus.lst
        packages-arch.lst
        packages-xtra.lst
        packages-xvid.lst
        packages-desk.lst
        packages-kids.lst
        packages-elec.lst
        packages-devl.lst
        packages-geog.lst
        packages-virt.lst
        packages-more.lst)
md5sums=('6cc44f2e394747fef5f6f82d05a94394'
         'a066b080604e036bcfb869a793e41416'
         '6f4654d88c5cc5ab4b3b02641f270bf9'
         '320d907116b1c7d566dd5161d492807b'
         '21c62b2872c7f4d71c47f286fa319680'
         '95d713e6b86e3a65ca67aeae6d7209b3'
         '7459c975d45c31e5aff451b61e3b10a7'
         'cecd4131d2129a2555f26e941b21be17'
         'b17a8d069ecc206adcfc56f38e6f72c7'
         '12c7b3a5e0167c9edbfd7819a25a7ab1'
         '828b607f5a5a7713b00a61214ff74906'
         '4cb1b6ab71e72e814972fff7fd16464c'
         'ac28f14da7e00d52b5d553100f82fcf7')

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

package_meta-unexicon-most() {
  pkgdesc="All unexicon meta packages"
  depends=('meta-unexicon' 'meta-unexicon-live' 'meta-unexicon-plus' 'meta-unexicon-arch' 'meta-unexicon-xtra' 'meta-unexicon-xvid' 'meta-unexicon-desk' 'meta-unexicon-elec' 'meta-unexicon-devl' 'meta-unexicon-geog' 'meta-unexicon-virt' 'meta-unexicon-more')
}

# vim:set ts=2 sw=2 et:
