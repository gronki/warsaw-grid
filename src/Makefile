
SCSSFLAGS := -C --sourcemap=none
cssdir = ../css

all: $(cssdir)/grid.css $(cssdir)/grid.min.css

$(cssdir)/%.css: %.scss _grid_core.scss
	scss --style expanded $(SCSSFLAGS) $<:$@
$(cssdir)/%.min.css: %.scss _grid_core.scss
	scss --style compressed $(SCSSFLAGS) $<:$@

clean:
	rm -f $(cssdir)/*.css
