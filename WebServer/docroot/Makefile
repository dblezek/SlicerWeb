######################################
%.html: %.haml
	haml -f html5 $^ $@
######################################
HTML= index.html

######################################
all: ${HTML}
	cd stylesheets; make
	cd remote; make
	cd remote/stylesheets; make

clean:
	rm -f ${HTML}
	cd stylesheets; make clean
	cd remote; make clean
	cd remote/stylesheets; make clean
