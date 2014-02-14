graphs:
	@echo Making all graphs into .svg files...
	@ls *.dot | sed s/.dot//g | awk '{print "dot -Tsvg -Kneato "$$1".dot -o "$$1".svg"}' | bash
	@ls *.dot | sed s/.dot//g | awk '{print "dot -Tps -Kneato "$$1".dot -o "$$1".ps"}' | bash
	@ls *.dot | sed s/.dot//g | awk '{print "dot -Tpng -Kneato "$$1".dot -o "$$1".png"}' | bash

clean:
	/bin/rm -f *.ps *.png
