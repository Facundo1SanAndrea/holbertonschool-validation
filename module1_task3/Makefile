build: ## creates the site
	hugo > /dev/null 2>&1

clean: ## clean the direcory
	rm -r dist/*

post: ## create post with given post_name and title
	hugo new posts/${POST_NAME}.md ; sed -i '/title/c\title: "${POST_TITLE}"' content/posts/${POST_NAME}.md

help: ## helps
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'