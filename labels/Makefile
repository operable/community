ifeq ($(GITHUB_AUTH_TOKEN),)
$(error The GITHUB_AUTH_TOKEN environment variable must be set!)
endif

run:
	docker run -v $(shell pwd)/config.toml:/etc/repo-gopher/config.toml -e GITHUB_AUTH_TOKEN=$(GITHUB_AUTH_TOKEN) ohaiwalt/repo-gopher
