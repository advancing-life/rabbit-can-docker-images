FROM debian:jessie

RUN apt-get update && \
			apt-get install -y \
				wget \
				gcc \
				make 

RUN wget https://cache.ruby-lang.org/pub/ruby/2.5/ruby-2.5.1.tar.gz && \
			tar zxvf ruby-2.5.1.tar.gz

WORKDIR /ruby-2.5.1

RUN ./configure && make && make install

CMD ["ruby", "-v"]
