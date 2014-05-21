---
layout: default
username: Differential
repo: meteor-blog
version: 0.4.3
desc: Gives you an basic, out-of-the-box blog at `/blog`

---
# Changelog

### v0.4.3

* Fix bug where LESS files were imported twice ([#48](https://github.com/Differential/meteor-blog/pull/48))
* Add support for `meteor-roles` groups

### v0.4.2

* Fix bugs with pagination ([#44](https://github.com/Differential/meteor-blog/issues/44)), author profile, and T9n.

### v0.4.0

_NOTE: In `0.4.0`, blog contents are stored as HTML, not markdown. There is an automatic migration step if you upgrade, but you may want to backup your blog posts first._

* Complete re-write of blog administrative interface
  * Replace Ace Editor with Medium Editor
  * Replace administrative blog list with fancy table
* Add Google+ authorship link to blog posts

### v0.3.0

_NOTE: `0.3.0` is not guaranteed to work with Meteor `0.7.x` and below. If you are using an older version of Meteor, use Blog `0.2.13`._

* Meteor `0.8.x` compatibility

### v0.2.12

* Add basic tagging of blog posts
* Save on publication data ([#33](https://github.com/Differential/meteor-blog/issues/33))
* Some preparations for Meteor Blaze

### v0.2.11

* Remove `parsleyjs` as a dependency
* Maintain package JS when user overrides view templates ([#28](https://github.com/Differential/meteor-blog/issues/28))
* Add keyboard shortcut to toggle `Preview` mode
* Ensure blog post slugs are unique
* Allow user to override admin templates ([#31](https://github.com/Differential/meteor-blog/issues/31))
* Tweak default CSS for blog list padding and blog post image margins

### v0.2.8

* Unnecessary code cleanup
* Remove hard dependency on moment.js version
* Rename method to minimize conflict
* Fix blog author in model
* Improve RSS

### v0.2.7

* Update to iron-router 0.6.2
* Fixed a few bugs (issues [#16](https://github.com/Differential/meteor-blog/issues/16) and [#17](https://github.com/Differential/meteor-blog/issues/17))
* Add server-side RSS feed

### v0.2.6

_NOTE: If you were using the `excerpt` helper before (`data.excerpt()`), it is now a field (`data.excerpt`)._

* Publish less data to blog index.
* Replace EpicEditor with Ace Editor
* Add simple 'Load More' pagination
* Turn admin roles off by default

### v0.2.5

* Support for fast-render, if your app is using it
* Ensure there is an index on the `slug` field for posts
* Hide draft posts from crawlers
* Improve FB share link
* Make default theme more narrow
* Require `blogAdmin` role to be allowed to admin posts

### v0.2.4

* Remove 'urlify2' package (was crashing phantomjs in production)

### v0.2.3

* Take out Bootstrap 3 files by default (user must add manually)
* Fix bug getting blog post thumbnail
* Publish only blog authors

### v0.2.2

* Fix bug where every blog author was 'Mystery author' on blog index page
* Fix sorting of blogs on index and admin pages
* Fix flash status message
* Rename 'user' model to 'author' (to help avoid conflicts)

### v0.2.1

* Rename 404 template
* Allow user to override package templates
* Add experimental handlebar helpers for blog content
* Fix a few bugs related to joining blog to author

### v0.2.0

_NOTE: `iron-router` 0.6.x is not backwards-compatible with earlier versions_

* Upgrade iron-router to 0.6.1 and minimongoid to 0.8.3
* Add 404 template
* Rename some files/folders to match http://github.com/Differential/meteor-boilerplate

### v0.1.0

* Initial release
