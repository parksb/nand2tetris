TARGET=build

test:
	make link file=$(file) ext=asm && cd $(TARGET) && CPUEmulator.sh $(file).tst

link:
	cd $(TARGET) && ln -sf ../$(file).$(ext)

link_all:
	make link file=* ext=cmp && make link file=* ext=tst

clean:
	rm $(TARGET)/*
