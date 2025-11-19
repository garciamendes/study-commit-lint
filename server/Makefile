project := server

run-setup-dev:
	pre-commit clean && \
	rm -rf ~/.cache/pre-commit && \
	pre-commit install --hook-type commit-msg && \
	pre-commit install && \
	pre-commit autoupdate

run-lint:
	pre-commit run --all-files

run-lint-fix:
	pre-commit run --all-files --hook-stage manual

create-commit: run-lint
	git add . && cz commit
