the following commands were used to extract the boot blocks from the minimyth2
images from https://github.com/warpme/minimyth2/releases

xzcat MiniMyth2-armv8-master-12.10.0.r1015-board-rk3566.x96_x6-SD-Image.img.xz | dd bs=512 of=boot-x96_x6.dd count=65535 seek=1 skip=1 status=progress
xzcat MiniMyth2-armv8-master-12.11.0.r1064-board-rk3566.quartz64-b-SD-Image.img.xz | dd bs=512 of=boot-quartz64-b.dd count=65535 seek=1 skip=1 status=progress
xzcat MiniMyth2-armv8-master-12.11.0.r1064-board-rk3566.rock3-c-SD-Image.img.xz | dd bs=512 of=boot-rock3-c.dd count=65535 seek=1 skip=1 status=progress
xzcat MiniMyth2-armv8-master-12.11.0.r1064-board-rk3568.rock3-a-SD-Image.img.xz | dd bs=512 of=boot-rock3-a.dd count=32767 seek=1 skip=1 status=progress
