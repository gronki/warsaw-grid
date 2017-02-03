
SCSSFLAGS := -C --sourcemap=none
cssdir = ../css

all: $(cssdir)/grid.css

$(cssdir)/%.css: %.scss _grid_core.scss
	scss --style compact $(SCSSFLAGS) $<:$@
$(cssdir)/%.min.css: %.scss _grid_core.scss
	scss --style compressed $(SCSSFLAGS) $<:$@

clean:
	rm -f $(cssdir)/*.css
