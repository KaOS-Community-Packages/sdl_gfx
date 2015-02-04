pkgname=sdl_gfx
pkgver=2.0.25
pkgrel=1
pkgdesc="SDL Graphic Primitives"
arch=('x86_64')
license=('LGPL')
url="http://www.ferzkopp.net/joomla/software-mainmenu-14/4-ferzkopps-linux-software/19-sdlgfx"
source=(http://www.ferzkopp.net/Software/SDL_gfx-2.0/SDL_gfx-${pkgver}.tar.gz)
depends=('sdl')
md5sums=('ea24ed4b82ff1304809c363494fa8e16')

build() {
  cd SDL_gfx-${pkgver}

    ./configure --prefix=/usr --disable-mmx

  make
}

package() {
  cd SDL_gfx-${pkgver}
  make DESTDIR=${pkgdir} install
} 
