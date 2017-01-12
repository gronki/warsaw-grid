
SCSSFLAGS := -C --sourcemap=none

cssdir = ../css

all: $(cssdir)/grid.css $(cssdir)/grid.min.css 

$(cssdir)/%.css: %.scss $(wildcard _*.scss)
	scss --style compact $(SCSSFLAGS) $<:$@
$(cssdir)/%.min.css: %.scss $(wildcard _*.scss)
	scss --style compressed $(SCSSFLAGS) $<:$@

clean:
	rm -f $(cssdir)/*.css
