#             __________               __   ___.
#   Open      \______   \ ____   ____ |  | _\_ |__   _______  ___
#   Source     |       _//  _ \_/ ___\|  |/ /| __ \ /  _ \  \/  /
#   Jukebox    |    |   (  <_> )  \___|    < | \_\ (  <_> > <  <
#   Firmware   |____|_  /\____/ \___  >__|_ \|___  /\____/__/\_ \
#                     \/            \/     \/    \/            \/
# $Id$
#
ROOT=../../..

CC = gcc
RM = rm -f

COMMON = main.c gd_bmp.c

INCLUDE = -I ../libwps/src \
          -I $(ROOT)/apps/gui \
          -I $(ROOT)/firmware/export \
          -I $(ROOT)/apps/recorder \
          -I $(ROOT)/apps \
          -I .

CFLAGS = -g -Wall

all:
	$(CC) $(INCLUDE) $(CFLAGS) $(COMMON) -rdynamic -ldl -lgd -lpng -o screenshot

clean:
	$(RM) screenshot
