# Illustration Instructions

Make a text file, named `illustration_your-last-name.txt`. Be sure it is *plain text* (make it in Atom (<https://atom.io>) or, if you use Word or GoogleDocs, be sure to save it as plain text.

You can download a [template file](https://github.com/Eumaeus/blackwell_fall_2018/blob/master/docs/illustration_template.txt) to get you started.

There are five "columns":

1. id
1. text-urn
1. rights
1. image-url
1. caption

The first line of the text file should name those columns:

> `https://github.com/Eumaeus/blackwell_fall_2018/blob/master/docs/illustration_template.txt`

Each subsequent line is a record that must consist of the same number of columns, and the columns should be divided by the character `#`.

- The `id` column should contain a value, unique in your list: your last name, an "`_`" character, and a number, from 1 to however many entries you make.
- The `text-urn` column should identify the passage of text you are illustrating. The identifier should look like `urn:cts:greekLit:tlg0016.tlg001.eng:1.6`, where `1.6` is the passage of Herodotus. **Make sure this is valid!** (see below)
- The `rights` column should contain a URL to a page where I can see that the image is licensed for re-use.
- The `image-url` column should contain a URL that takes me to the image, ideally just the image.
- The `caption` column is where you describe what the image is and how it illustrates the passage. Here is where you may choose to be creative.

You may have more than one illustration for the same cited passage. For example, 1.6 might have an illustration of Croesus and of the river Halys. Each of those will have a unique `id`, but the same `text-urn`. Put the entries in the sequence you want (so here, Croesus would come before Halys in the list.)

## How to validate a URN

Go to <http://folio.furman.edu/herodotus.html> and paste a Herodotus URN into the URN field in the upper-left of the screen. Click "Retrieve Passage". If you see the passage of Herodotus, it is a valid URN. The web-app will tell you if it not valid. **This is the important thing to get right.**

