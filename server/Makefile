project := server

run-setup-dev:
	pre-commit clean && \
	rm -rf ~/.cache/pre-commit && \
	pre-commit install --hook-type commit-msg && \
	pre-commit install && \
	pre-commit autoupdate
