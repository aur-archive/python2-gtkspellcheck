# Maintainer: Maximilian Köhl <linuxmaxi@googlemail.com>
pkgname=python2-gtkspellcheck
pkgver=4.0
pkgrel=1
pkgdesc="A simple but quite powerful spellchecking library written in pure Python for Gtk based on Enchant."
arch=(any)
url="http://koehlma.github.com/projects/pygtkspellcheck.html"
license=('GPL')
depends=('python2-pyenchant')
makedepends=('python2-sphinx')
optdepends=('gtk3: gtk 3 bindings'
            'gtk2: gtk 2 bindings'
            'pygtk: gtk 2 pygtk bindings'
            'python2-gobject: gtk 2 and 3 gi bindings')
conflicts=('python2-gtkspell')
provides=('python2-pylocales' 'python2-gtkspell')
replaces=('python2-gtkspell')
source=(https://github.com/koehlma/pygtkspellcheck/tarball/v${pkgver})
md5sums=('44da8d279f5e9628a38edb2cad69e8e1')

build() {
    cd koehlma-pygtkspellcheck-*
    export GTKSPELL=true
    python2 setup.py install --root=${pkgdir}
}

