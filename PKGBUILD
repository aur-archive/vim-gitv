pkgname=vim-gitv
pkgver=1.1
pkgrel=2
pkgdesc="gitk for Vim"
arch=('any')
url="http://www.vim.org/scripts/script.php?script_id=3574"
license=('custom:vim')
groups=('vim-plugins')
depends=('vim-runtime>=7.2' 'git' 'vim-fugitive')
makedepends=()
install=vimdoc.install
source=('http://www.vim.org/scripts/download_script.php?src_id=16307')
md5sums=('ca8cbf1585d94c6d8e4e58ac7288f4e4')

package() {
    cd "$srcdir/gitv-$pkgver"
    installpath="$pkgdir/usr/share/vim/vimfiles"
    install -Dm644 doc/gitv.txt      $installpath/doc/gitv.txt
    install -Dm644 plugin/gitv.vim   $installpath/plugin/gitv.vim
    install -Dm644 ftplugin/gitv.vim $installpath/ftplugin/gitv.vim
    install -Dm644 syntax/gitv.vim   $installpath/syntax/gitv.vim
}
