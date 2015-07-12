FROM debian:jessie
MAINTAINER Steve Domin <steve@stevedomin.com>

RUN apt-get update && apt-get install -y wget

RUN echo "deb http://packages.erlang-solutions.com/debian jessie contrib" >> /etc/apt/sources.list
RUN wget http://packages.erlang-solutions.com/ubuntu/erlang_solutions.asc && apt-key add erlang_solutions.asc

RUN apt-get update && apt-get install -y \
  erlang=1:17.5.3 erlang-base-hipe=1:17.5.3 erlang-dev=1:17.5.3 erlang-appmon=1:17.5.3 \
  erlang-asn1=1:17.5.3 erlang-common-test=1:17.5.3 erlang-corba=1:17.5.3 erlang-crypto=1:17.5.3 erlang-debugger=1:17.5.3 \
  erlang-dialyzer=1:17.5.3 erlang-edoc=1:17.5.3 erlang-erl-docgen=1:17.5.3 erlang-et=1:17.5.3 erlang-eunit=1:17.5.3 \
  erlang-gs=1:17.5.3 erlang-ic=1:17.5.3 erlang-inets=1:17.5.3 erlang-inviso=1:17.5.3 erlang-megaco=1:17.5.3 \
  erlang-mnesia=1:17.5.3 erlang-observer=1:17.5.3 erlang-odbc=1:17.5.3 erlang-os-mon=1:17.5.3 erlang-parsetools=1:17.5.3 \
  erlang-percept=1:17.5.3 erlang-pman=1:17.5.3 erlang-public-key=1:17.5.3 erlang-reltool=1:17.5.3 \
  erlang-runtime-tools=1:17.5.3 erlang-snmp=1:17.5.3 erlang-ssh=1:17.5.3 erlang-ssl=1:17.5.3 erlang-syntax-tools=1:17.5.3 \
  erlang-test-server=1:17.5.3 erlang-toolbar=1:17.5.3 erlang-tools=1:17.5.3 erlang-tv=1:17.5.3 erlang-typer=1:17.5.3 \
  erlang-webtool=1:17.5.3 erlang-wx=1:17.5.3 erlang-xmerl=1:17.5.3 erlang-diameter=1:17.5.3 erlang-eldap=1:17.5.3

CMD ["erl"]
