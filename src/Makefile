
cssdir = ../css
deps = _respond.sass

all: $(cssdir)/grid.css $(cssdir)/grid.min.css

$(cssdir)/grid.css: grid.sass $(deps)
	sass --no-cache --sourcemap=none --style expanded $<:$@

$(cssdir)/grid.min.css: grid.sass $(deps)
	sass --no-cache --sourcemap=none --style compressed $<:$@

$(cssdir)/%.css.gz: $(cssdir)/%.css
	gzip -f $<

clean:
	rm -f $(cssdir)/*.css $(cssdir)/*.gz
