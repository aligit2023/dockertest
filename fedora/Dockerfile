FROM	aligit2023/c3c_build_base_fedora
WORKDIR	/opt
RUN	git clone https://github.com/c3lang/c3c.git --depth 1
RUN	cd c3c && mkdir build && cd build && cmake ..
RUN	cd c3c/build && cmake --build .
RUN	mv c3c/build c3c_binary_fedora
RUN	tar czvf c3c_binary_fedora.tar.gz c3c_binary_fedora
CMD	["sh"]
