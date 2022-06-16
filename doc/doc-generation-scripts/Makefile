all: generate

prepare:
	pip install json-schema-for-humans

generate:
	rm -rf ./tmp
	mkdir tmp
	generate-schema-doc --config-file doc-format-config.json ../../schemas/feasibility ./tmp
	cp merge-md-step1.json tmp/manifest.json && cd tmp && npx merge-markdown
	npx merge-markdown -m merge-md-step2.json
	npx merge-markdown -m merge-md-step3.json
	rm -rf ./tmp
	mdpdf ../Readme.md

.PHONY: prepare generate
