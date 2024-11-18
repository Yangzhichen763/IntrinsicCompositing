运行下列指令之前要先将 BoostingMonocularDepth, intrinsic, omnidata 三个包安装到本地，并将报下的 setup.py 中的 github.com 链接改为 gitclone.com/github.com
```shell
git clone https://github.com/CCareaga/omnidata src/omnidata
git clone https://github.com/compphoto/intrinsic src/intrinsic
git clone https://github.com/CCareaga/BoostingMonocularDepth src/BoostingMonocularDepth
```
使用 gitclone.com/github.com 链接安装依赖包的目的在于避免由于网络问题导致安装失败。
```shell
pip install git+https://gitclone.com/github.com/CCareaga/MiDaS@master
pip install git+https://gitclone.com/github.com/CCareaga/chrislib@main

cd src/BoostingMonocularDepth/
pip install .
cd ..

cd src/intrinsic/
pip install .
cd ..

cd src/omnidata/
pip install .
cd ..
```