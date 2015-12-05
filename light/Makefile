.PHONY:clean
main.bin:main.ihx
	objcopy -I ihex -O binary main.ihx main.bin

main.ihx:main.c
	sdcc -I. -mmcs51 main.c -o main.ihx
clean:
	rm -f main.bin main.ihx main.rel main.sym main.asm main.lk main.lst 
	rm -f main.map main.rst main.mem
