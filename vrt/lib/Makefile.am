#
# Copyright 2007,2008,2009 Free Software Foundation, Inc.
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.
#

include $(top_srcdir)/Makefile.common

AM_CPPFLAGS = \
    $(VRT_INCLUDES) \
    $(BOOST_CPPFLAGS) \
    $(CPPUNIT_INCLUDES) \
    $(GRUEL_INCLUDES)

bin_PROGRAMS = 

lib_LTLIBRARIES = \
	libvrt.la

libvrt_la_SOURCES = \
	copiers.cc \
	data_handler.cc \
	expanded_header.cc \
	rx.cc \
	rx_packet_handler.cc \
	socket_rx_buffer.cc

libvrt_la_LIBADD =

# Private headers not needed for above the API development
noinst_HEADERS = \
	data_handler.h \
	expanded_header_parse_switch_body.h \
	expanded_header_unparse_switch_body.h \
	socket_rx_buffer.h

EXTRA_DIST = \
	gen_parse_switch_body.py \
	gen_unparse_switch_body.py
