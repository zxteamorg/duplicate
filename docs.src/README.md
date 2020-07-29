# Knowledge Base

## Developing
1. Update repo
	```bash
	git pull --rebase
	git lfs fetch
	```
1. Start development server
	```bash
	docker build --tag duplicate --file docker/Dockerfile . && docker run --interactive --tty --rm --name duplicate --volume $(pwd):/development --publish 8000:8000 duplicate
	```
1. Open browser http://127.0.0.1:8000/
1. Edit content of `src/` and look for hot-reloaded changes in the browser
