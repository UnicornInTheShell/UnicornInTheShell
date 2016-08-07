---
layout: post
title: jekyll helpful gems
---

After switching to Jekyll for simplicity, I went back to look for some helpful (not so clutering) libraries (aka rub gems) that can faciliate with posting faster.

Here is the list:

	* `gem 'jemoji'`
	* `gem 'jekyll-seo-tag'`
	* `gem 'jekyll-gist'`
	* `gem 'jekyll-feed'`
	* `gem 'jekyll-compose', group: [:jekyll_plugins]`:
		* This one is my favourite, it offer commands like:


		```
		draft      # Creates a new draft post with the given NAME
		post       # Creates a new post with the given NAME
		publish    # Moves a draft into the _posts directory and sets the date
		unpublish  # Moves a post back into the _drafts directory
		page       # Creates a new page with the given NAME

		$ bundle exec jekyll page "My New Page"
		$ bundle exec jekyll post "My New Post"
		$ bundle exec jekyll draft "My new draft"


		$ bundle exec jekyll publish _drafts/my-new-draft.md
		# or specify a specific date on which to publish it
		$ bundle exec jekyll publish _drafts/my-new-draft.md --date 2014-01-24

		$ bundle exec jekyll unpublish _posts/2014-01-24-my-new-draft.md

		```
