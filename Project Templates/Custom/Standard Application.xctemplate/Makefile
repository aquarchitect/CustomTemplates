SCRIPT = ~/Documents/X-code/Scripting.playground/generate_appicons.swift

JSON = Contents.json
PDF = ___PACKAGENAME___.pdf

appicons: $(JSON) $(PDF)
	@ swift $(SCRIPT) $(PDF) $(JSON)

clean: *.png
	@ rm $(SOURCE)/*.png