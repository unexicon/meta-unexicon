# Maintainer: Brian Bidulock <bidulock@openss7.org>
pkgname=(
    'meta-unexicon'
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
    'meta-unexicon-most')
pkgbase='meta-unexicon'
pkgver=1.1
pkgrel=21
pkgdesc="A collection of meta packages for the unexicon distribution"
arch=('any')
url="http://www.unexicon.com"
license=('GPL')
groups=('unexicon')
depends=()
depends=(`cat packages-live.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-plus.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-arch.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-xtra.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-xvid.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-desk.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-kids.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-elec.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-devl.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-geog.lst|sed -r 's,[[:space:]]*#.*,,'`
         `cat packages-virt.lst|sed -r 's,[[:space:]]*#.*,,'`)
source=(packages-live.lst
        packages-plus.lst
        packages-arch.lst
        packages-xtra.lst
        packages-xvid.lst
        packages-desk.lst
        packages-kids.lst
        packages-elec.lst
        packages-devl.lst
        packages-geog.lst
        packages-virt.lst)
md5sums=('f254fab80f43027ae4ac64723f56266d'
         'a227fae577d5bbb9880b6aa64eeea8c1'
         '9f09c618b12c9fd9db5972a733570315'
         '62ab3c02887d062afba7d23489dae7f1'
         '415941127fce09f5a1267d43eb53bcc6'
         '067d3fb6e82efc02c860e2b642596aa1'
         '382886c299d9bf081619ac5a8db84ac5'
         'b51afaef3e16baca631316f57f7ac2f2'
         '52e7f85dc4ec6a103734758bbc975150'
         '53213aea84be024b81efb2135ace74d1'
         '00ffa8c520a320e62ca9a2a73a00c645')

package_meta-unexicon() {
  pkgdesc="A meta package for unexicon (remove me)"
  depends=()
  install -Dm644 <(echo "") "$pkgdir/usr/share/unexicon/installed/meta-unexicon"
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

package_meta-unexicon-most() {
  pkgdesc="All unexicon meta packages"
  depends=('meta-unexicon' 'meta-unexicon-live' 'meta-unexicon-plus' 'meta-unexicon-arch' 'meta-unexicon-xtra' 'meta-unexicon-xvid' 'meta-unexicon-desk' 'meta-unexicon-kids' 'meta-unexicon-elec' 'meta-unexicon-devl' 'meta-unexicon-geog' 'meta-unexicon-virt')
}

# vim:set ts=2 sw=2 et:
