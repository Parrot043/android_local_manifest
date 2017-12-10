Local manifest for Jiayu s3 (Lineage os 15.0) 

Getting Started

Initialize a repository with LineageOS:

repo init -u git://github.com/LineageOS/android.git -b lineage-15.0

Copy "mtk.xml" under android_src/.repo/local_manifests

repo sync -j7

Build the code:

source build/envsetup.sh

breakfast s3_h560

make -j4 bacon showcommands 2>&1 | tee build.log

