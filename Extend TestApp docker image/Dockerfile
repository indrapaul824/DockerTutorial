FROM indrap24/testimagerepo:hubtest

RUN apk update && apk upgrade

RUN apk add --no-cache bash\
                       python \
                       pkgconfig \
                       git \
                       gcc \
                       openldap \
                       libcurl \
                       python2-dev \
                       gpgme-dev \
                       libc-dev \
    && rm -rf /var/cache/apk/*

RUN pip install --upgrade pip

RUN pip3 install NLTK