# pdf2png
Shell tool to transform pdf files to png files.

# Install
1. Use git clone to download the package.
```shell
git clone git@github.com:xingzhou1002/pdf2png
```
2. Install dependencies
```shell
conda install pymupdf
```
or
```shell
pip install pymupdf
```

3. Use makepkg to install the package.Make sure that the path is right. 
```shell
cd ./pdf2png
makepkg -si
```

Also you can use nuitka to compile.
```shell
cd ./src
nuitka \
  --onefile \
  --standalone \
  --remove-output \
  --lto=auto \
  --enable-plugin=pyqt5 \
  pdf2png.py
```
Then install by
```shell
sudo install -Dm755 ./src/pdf2png "$pkgdir/usr/bin/pdf2png"                
```

# Use
Use "pdf2png" commend to this package.
For sigle pdf file.
Use
```shell
pdf2png xxx.pdf
```
For pdfs in a dir.
USE
```shell
pdf2png path_to_dir
```
If you want to trasform all the pdf in the local path.
Use
```shell
pdf2png .
```