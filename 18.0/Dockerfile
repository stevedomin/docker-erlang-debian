FROM debian:jessie
MAINTAINER Steve Domin <steve@stevedomin.com>

RUN apt-get update && apt-get install -y wget

RUN echo "deb http://packages.erlang-solutions.com/debian jessie contrib" >> /etc/apt/sources.list
RUN wget http://packages.erlang-solutions.com/ubuntu/erlang_solutions.asc && apt-key add erlang_solutions.asc

RUN apt-get update && apt-get install -y \
  erlang=1:18.0 erlang-base-hipe=1:18.0 erlang-dev=1:18.0 erlang-appmon=1:18.0 \
  erlang-asn1=1:18.0 erlang-common-test=1:18.0 erlang-corba=1:18.0 erlang-crypto=1:18.0 erlang-debugger=1:18.0 \
  erlang-dialyzer=1:18.0 erlang-edoc=1:18.0 erlang-erl-docgen=1:18.0 erlang-et=1:18.0 erlang-eunit=1:18.0 \
  erlang-gs=1:18.0 erlang-ic=1:18.0 erlang-inets=1:18.0 erlang-inviso=1:18.0 erlang-megaco=1:18.0 \
  erlang-mnesia=1:18.0 erlang-observer=1:18.0 erlang-odbc=1:18.0 erlang-os-mon=1:18.0 erlang-parsetools=1:18.0 \
  erlang-percept=1:18.0 erlang-pman=1:18.0 erlang-public-key=1:18.0 erlang-reltool=1:18.0 \
  erlang-runtime-tools=1:18.0 erlang-snmp=1:18.0 erlang-ssh=1:18.0 erlang-ssl=1:18.0 erlang-syntax-tools=1:18.0 \
  erlang-test-server=1:18.0 erlang-toolbar=1:18.0 erlang-tools=1:18.0 erlang-tv=1:18.0 erlang-typer=1:18.0 \
  erlang-webtool=1:18.0 erlang-wx=1:18.0 erlang-xmerl=1:18.0 erlang-diameter=1:18.0 erlang-eldap=1:18.0

CMD ["erl"]
