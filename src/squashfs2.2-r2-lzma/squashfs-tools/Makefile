INCLUDEDIR = .
LZMADIR = ./lzma/C

CFLAGS := -I$(INCLUDEDIR) -I$(LZMADIR) -D_FILE_OFFSET_BITS=64 -D_LARGEFILE_SOURCE -g

mksquashfs: mksquashfs.o read_fs.o sort.o
	$(CC) $(LZMADIR)/Alloc.c $(LZMADIR)/LzFind.c $(LZMADIR)/LzmaEnc.c $(LZMADIR)/LzmaDec.c $(LZMADIR)/LzmaLib.c mksquashfs.o read_fs.o sort.o -lz -o $@

mksquashfs.o: mksquashfs.c mksquashfs.h

read_fs.o: read_fs.c read_fs.h

sort.o: sort.c
