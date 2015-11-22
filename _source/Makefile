# You must have jekyll and R installed, and they must be in PATH. For R, you
# need to install the servr package.

all:
	Rscript -e "servr::jekyll(input = c('..', '../_source/articles', '../_source/blog'), output = c('..', '../_posts/articles', '../_posts/blog'))"

clean:
	rm -r ../_site