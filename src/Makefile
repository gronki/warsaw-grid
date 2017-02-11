
cssdir = ../css

all: $(cssdir)/grid.css

$(cssdir)/%.css: %.sass _respond.sass
	sass --style compact $<:$@

clean:
	rm -f $(cssdir)/*.css
