MAINTAINERCLEANFILES = $(srcdir)/Makefile.in

CLEANFILES = test*.log test*.trs \
  *.pcap-dist \
  dns.out \
  no-layers.out layers.out \
  frags.out \
  padding-no-layers.out padding-layers.out \
  vlan11.out \
  dnspad.out \
  test7.out test7.layer.out \
  test8.out \
  test9.out \
  test10.out \
  test11.out \
  test12.out test12.20161020.152301.075993.gz \
  test13.out \
  test14.out

TESTS = test1.sh test2.sh test3.sh test4.sh test5.sh test6.sh test7.sh \
  test8.sh test9.sh test10.sh test11.sh test12.sh test13.sh test14.sh

test1.sh: dns.pcap-dist

test2.sh: dns.pcap-dist

test3.sh: frags.pcap-dist

test4.sh: 1qtcppadd.pcap-dist

test5.sh: vlan11.pcap-dist

test6.sh: dnspad.pcap-dist

test7.sh: 1qtcpnosyn.pcap-dist dnso1tcp.pcap-dist \
  do1t-nosyn-1nolen.pcap-dist dnso1tcp-midmiss.pcap-dist

test8.sh: dnsotcp-many1pkt.pcap-dist dnsotcp-manyopkts.pcap-dist \
  dnso1tcp-bighole.pcap-dist

test9.sh: dns.pcap-dist

test10.sh: dns6.pcap-dist

test11.sh: dns.pcap-dist

test12.sh: dns.pcap-dist

test13.sh: dns.pcap-dist

test14.sh: dns.pcap-dist

.pcap.pcap-dist:
	cp "$<" "$@"

EXTRA_DIST = $(TESTS) \
  dns.gold dns.pcap \
  frags.pcap \
  1qtcppadd.pcap \
  vlan11.gold vlan11.pcap \
  dnspad.gold dnspad.pcap \
  test7.gold 1qtcpnosyn.pcap dnso1tcp.pcap do1t-nosyn-1nolen.pcap \
  dnso1tcp-midmiss.pcap \
  test8.gold dnsotcp-many1pkt.pcap dnsotcp-manyopkts.pcap \
  dnso1tcp-bighole.pcap \
  test9.gold \
  dns6.pcap test10.gold \
  test14.gold
