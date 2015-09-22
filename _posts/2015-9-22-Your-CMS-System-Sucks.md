---
layout: post
title: Your CMS System Sucks
---

# Your CMS System Sucks

The first rule of content management systems is that you’re using the wrong one. Using Wordpress? You’re a fifth-grader running a coloring-contest blog. Drupal? You should be using Wordpress. An enterprise solution? You’re an open-source Judas.

This is often how it feels, at least, if you hang around the rough parts of the web-dev Twitter or loiter in blog comments. The real first rule of content management systems is that it's not so much which CMS you use as *how* you use it.

I'm going to ruin your day by presenting a quote from Frydor Dostoyevsky:

  > Man is tormented by no greater anxiety than to find someone quickly to whom he can hand over that great gift of freedom with which the ill-fated creature is born.
  
Dostoyevsky meant that the nicest thing you can tell your CMS users is that they don’t have the freedom to mess things up. When implementing a CMS, try to give your users exactly the level of freedom they need—but, when in doubt, err on the side of giving them slightly too much. Remember, a bottom-drawer CMS implemented with care will often be much more useful than a top-drawer system pulled straight out of the box and shoved onto your server.

If you're thinking about CMS implementation, you're probably in of two situations:

1. You're creating a new site and world is your CMS-implementation oyster
2. You're managing or refurbishing an existig site and the CMS setup brings you great sadness.

### Can this element have its own field?

With many content management systems, content types come default with a big text field where anything can be entered. Consider limiting this freedom as much as possible by giving discrete elements discrete inputs. Every element that serves a purpose distinct from other elements should have its own input field.

For those who think partitioning every element into its own field is excessive, remember that it gives you flexibility in the future. In a staff directory, a person's job title and name ought to have separate input fields. The same goes for photo, office hours, and contact info, even though they appear next to each other on the page.

### Can this field be more restrictive?

It's a good idea to use the most restrictive field you can for an element. Restricting fields makes it easier for the people using the CMS to do their jobs correctly and quickly, and it can also help bring an editorial and visual consistency to the site. Having users select the day of the week from an array instead of typing it into a text field ensures that all days of the week will always be spelled correctly.

Restricting fields is also one of the most significant ways you can let CMS users know that they can’t mess things up. By using a restricted image field, you implicitly assure people that if they try to upload the wrong type of image file, the CMS will reject it.

### Does the user need this permission?

Restricting a user's permissions is the easiest way to make sure they can't accidentally destroy the site. Most content editors won't need to mess around with permalinks, so don't give them permission to do so. If a user is only editing existing content, you should avoid giving them permission to create or delete pages.

To figure out what permissions users actually need: create a new user and turn off all permissions. Log in as that user and go about accomplishing all the tasks that user will need to do and add permissions to that account as needed.

### Okay, great - but what about politics?

For most web-development situations, the technical part will likely be easier than the political part. How do you sell the client or your boss on spending an extra week or so on making the CMS better? It's not only possible to get approval to spend time on this, but you can get outright gratitude.

If that doesn't work, here are a few sound bites you can use"
  * “This is a special, one-of-a-kind organization, so we need to spend a little more time making sure the CMS meets its unique needs.”
  * “You have talented staff doing important work, and we don’t want them to have to spend their valuable time troubleshooting errors on the website.”
  * “We want to make sure there’s no way you can do anything to mess up the site. That way you’ll never have to pay us again.”
  * “See this page where someone uploaded a dog GIF and typed some flashing red text? I can prevent that from ever happening again.”

