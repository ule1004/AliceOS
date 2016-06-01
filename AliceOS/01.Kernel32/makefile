all: Kernel32.bin

VirtualOS.bin: VirtualOS.asm
	nasm -o VirtualOS.bin VirtualOS.asm
	
Kernel32.bin: Source/EntryPoint.s
	nasm -o Kernel32.bin $<
	
clean:
	rm -f VirtualOS.bin
	rm -f Kernel32.bin
