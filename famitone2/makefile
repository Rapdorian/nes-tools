CC = gcc

build: bin/text2data bin/nsf2data bin/nesasmc

install: build 
	mv bin/* ~/.local/bin

clean:
	rm bin -r

bin:
	mkdir bin

bin/%: %.cpp bin
	$(CC) $< -o $@

