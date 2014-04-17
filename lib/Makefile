STATICLIB = libimagequant.a
OBJS = pam.o mediancut.o blur.o mempool.o viter.o nearest.o libimagequant.o

all: static

static: $(STATICLIB)

$(STATICLIB): $(OBJS)
	$(AR) $(ARFLAGS) $@ $^

$(OBJS): pam.h

clean:
	rm -f $(OBJS) $(STATICLIB)

.PHONY: all static clean
.DELETE_ON_ERROR:
