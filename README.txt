## Drupal Static

To be clear, this is just an idea at this point. I'm going to be playing a bit more to see how I can get it working.

### What is this?

 This is a script that helps to export a Drupal site to a static site.

### Doesn't this already exist?

 Kinda. It exists in the form of Boost and perhaps a few other modules.

### What's the diff?

 This script looks to take your site and build out the directory structure
 that your current site uses but it converts everything to HTML pages instead.

### How's it work?

 Well it doesn't work YET (@TODO Update this when it works)

### How will it work.

 There are a couple options
 - full site build
   This does what you'd expect, spider the whole site and create the layout

 - latest updates
   There is a variable set in by the script called last_static. This script
   checks the updates for those pages that have either been updated, or 
   created since this last_static timestamp. If the page is published, it will
   be redownloaded to the deployment directory.

 - single page
   This script isn't perfect yet so pages that are run by views don't have a
   nice URL using /node/1234 associated to them, so these pages can be submitted
   individually.

### But this is a crappy way to do it.
 This spawned out of discussions with a few friends about static site generators
 and while this may not be the best (or even a good) way to do it, I created
 it to see where I could go with it. I'm very open to other ideas!

