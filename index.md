---
title: Docs
---
# A site for an Anti-Barclays Manchester group

_[sharklays.gq](http://sharklays.gq/)_

## Set up

* Registered the **[sharklays.gq](http://sharklays.gq/)** domain with [Free Nom](https://www.freenom.com)

![](/images/domain-freenom.png)

* Set up hosting with a Hostinger plan I already had in use
* Installed the latest WordPress version through SSH:

```sh
$ cd domains/sharklays.gq
$ cd public_html
$ rm -R *
$ wget http://wordpress.org/latest.tar.gz
$ tar xfz latest.tar.gz
$ ls
latest.tar.gz  wordpress
$ cp -r wordpress/* ./
```

* Set up the database through the Hostinger's MySQL interface
* Edited the wp-config.php file to add new database information
* Finished the setup through the WordPress interface.

![](/images/wordpress-install.png)



## Design principles

This site is for a small group with limited resources, so making sure that it
is as hassle free to edit and maintain is important. It is important that the
Action Network form just works and could be easily changed if the group decided to.

It was for that reason I decided to use the **original** embed code:

```html
<link
  href='https://actionnetwork.org/css/style-embed-v3.css'
  rel='stylesheet'
  type='text/css' />
<script
  src='https://actionnetwork.org/widgets/v4/letter/help-us-stop-barclays-from-fuelling-the-climate-crisis?format=js&source=widget'>
</script>
<div
  id='can-letter-area-help-us-stop-barclays-from-fuelling-the-climate-crisis'
  style='width: 100%'>
  <!-- this div is the target for our HTML insertion -->
</div>
```

With the width set to fill all the available space on the page.

Although there is a temptation to write custom CSS to style the form, the original
styling and form design is complex enough for inevitable bugs and pitfalls that
would not be easily manageable by a small low capacity group. Hence, the original
embed code.

### Branding

I did my best to mirror the branding of [Sharklays](https://sharklays.co.uk/).
For example, taking this logo:

![Pic of 2 sharks and SHARKLAYS written after](/images/sharklayslogo-nodrop.png)

And modifying it to be more relevant to the group:

![Pic of 2 sharks and SHARKLAYS MANCHESTER written after](/images/sharklayslogo-nodrop-mcr.png)

The rest of the site uses a standard WordPress theme with Barclays blue highlights.

### Accessibility

The most import part of web design, and content management.

#### Users

The site is small and being an off-the-shelf theme the general accessibility
of the site should be okay.

Where relevant, I have added alternative text to images.

#### Content managers

WordPress is the most comment Content Management Service (CMS), so should be the
most likely tool people would be familiar with. Had the group shown no previous
experience managing websites another CMS (possibly GIT or API driven) could be
just as appropriate.

## Real life

If this was a real life scenario, then ideally at least a quick phone call with
the group would be useful. I would ask them to put a document together with some
content, some ideas about what else the site could be used for and at slight vision of
it purpose.

Once the site had some content and the basic functionality, another phone call with
the person taking on managing the site to go over signing in and editing.

Assuming website creation and management to be part of a general digital
toolkit, this should be followed by sending links to the documentation for how to manage
a WordPress site for activists so they have a reference for when things,
inevitably, go wrong!

Finally, making sure that the person in the Manchester group has a number to call
or place to contact if things go terribly wrong and the documentation doesn't help.
Whether that would be me, or someone in in a nearby group with the knowledge to help
would depend on the circumstances.
