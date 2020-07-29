# alphachai/isort

```bash
# check
docker run -it --rm --mount type=bind,src=$(pwd),dst=/app alphachai/isort $(ISORT_FLAGS) --check-only $(PYTHON_LINT_TARGETS) --diff

# format
docker run -it --rm --user $(id -u):$(id -g) --mount type=bind,src=$(pwd),dst=/app alphachai/isort $(ISORT_FLAGS) $(PYTHON_LINT_TARGETS)
```
