FROM gcc

RUN git clone https://github.com/Exter-N/seqgend.git \
    && cd /seqgend \
    && make \
    && make install


COPY seqgend.conf /etc/seqgend.conf

EXPOSE 65279/udp
CMD /usr/sbin/seqgend
