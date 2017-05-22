FROM tpdock/alpine-elixir:1.4.2-otp18

RUN apk --update add erlang-crypto erlang-syntax-tools erlang-parsetools \
      erlang-inets erlang-ssl erlang-public-key erlang-eunit erlang-xmerl \
      erlang-edoc erlang-tools erlang-mnesia erlang-runtime-tools musl-dev \
      erlang-asn1 erlang-sasl erlang-erl-interface erlang-dev \
      gcc wget git openssh make bash grep && \
    rm -rf /var/cache/apk/* && \
    mix local.hex --force && \
    mix local.rebar --force
