FROM silviubadragan/base

RUN wget https://dl.google.com/go/go1.13.6.linux-amd64.tar.gz \
    && tar -C /usr/local -xzf go1.13.6.linux-amd64.tar.gz \
    && rm -r go1.13.6.linux-amd64.tar.gz

ENV PATH="/usr/local/go/bin:${PATH}"
