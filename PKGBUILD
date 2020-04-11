pkgname=slock
gitname=slock
pkgver=1.4
pkgrel=1
pkgdesc='Locker for X11'
arch=('x86_64')
source=('git+https://github.com/SearyBlue/slock')
sha1sums=('SKIP')
provides=('slock')
conflicts=('slock' 'slock-git')
build() 
{
	cd "$srcdir/$gitname"
	make
}

package() 
{
  	cd "$srcdir/$gitname"
  	make PREFIX=/usr DESTDIR="${pkgdir}" install
}
