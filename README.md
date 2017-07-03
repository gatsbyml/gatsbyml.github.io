# Gatsby MLJC web site

This is the repository for Gatsby Machine Learning Journal Club's web site at
[https://gatsbyml.github.io](https://gatsbyml.github.io/). The web site is
implemented with [Jekyll](https://jekyllrb.com) using [Github
pages](https://pages.github.com) as its host. The repository was set up by [Wittawat Jitkrittum](http://wittawat.com).


To MLJC coordinators:

* Clone the repository. Test the web site locally with your local Jekyll installation before you push. You can preview the generated site locally with 

    jekyll serve -P 7000 --watch

This will start a local web server allowing you to view the site at
`http://localhost:7000`. Read about it [here](https://jekyllrb.com/docs/usage/).

* Every git push will automatically trigger Jekyll's rebuild. The web site will
  be updated within a few seconds.

* Make sure that you update the web site at least once a week. Be sure to add a new
  entry after every talk. Ask the presenter for the slides and upload them to
  the site as well. If the presenter used whiteboard, take the photo of the
  board and upload the photo.

* Event data are stored in `_data/events.yml`. To update, just add the new YAML
  entry. You should be able to guess how to do so by see the past entries.
  The front page is, by default, configued to show these entries automatically
  as a big table. 


