TARGET=build

test:
	make link ext=asm && cd $(TARGET) && CPUEmulator.sh Mult.tst

link:
	cd $(TARGET) && ln -sf ../Mult.$(ext)

link_all:
	make link ext=cmp && make link ext=tst

clean:
	rm $(TARGET)/*
