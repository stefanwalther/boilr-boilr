help:														## Show this help.
	@echo ''
	@echo 'Available commands:'
	@grep -E '^[a-zA-Z0-9_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
	@echo ''
.PHONY: help

gen-readme: gen-output					## Generate README.md (using docker-verb)
	docker run --rm -v ${PWD}:/opt/verb stefanwalther/verb
.PHONY: gen-readme

gen-output: reg      						## Generate the sample output
	mkdir -p ./sample ; \
	cd ./sample; \
	boilr template use {{TemplateTag}} .; \
	tree -a > ./../docs/boilr-output.md; \
	cd ..; \
	rm -rf ./sample;
.PHONY: gen-output

reg:														## Register the current template locally
	boilr template save $(PWD) {{TemplateTag}} -f
.PHONY: reg


