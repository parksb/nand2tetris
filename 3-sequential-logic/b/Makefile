TARGET=build

test:
	make link chip=$(chip) ext=hdl && cd $(TARGET) && HardwareSimulator.sh $(chip).tst

link:
	cd $(TARGET) && ln -sf ../$(ext)/$(chip).$(ext) .

link_all:
	make link chip=* ext=cmp && make link chip=* ext=tst

clean:
	rm $(TARGET)/*
