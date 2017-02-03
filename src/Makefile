
SCSSFLAGS := -C --sourcemap=none
cssdir = ../css

all: $(cssdir)/grid.css

$(cssdir)/%.css: %.scss _respond.scss
	scss --style compact $(SCSSFLAGS) $<:$@

clean:
	rm -f $(cssdir)/*.css
