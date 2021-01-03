# Calalinaでは動作せず Bad CPU type
run :
	../../z_tools/nask helloos.nas helloos.img
	cp helloos.img ../../z_tools/qemu/fdimage0.bin
	make -C ../../z_tools/qemu


build_image :
	nasm helloos.nas -o helloos.img

run_image :
	qemu-system-i386 -drive file=helloos.img,format=raw,if=floppy -boot a