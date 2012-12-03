Adding images to the Collections Browser hierarchy
==================================================

Images can be added to any node that will appear in the online Collections Browser
hierarchy by using the Thesaurus Editor to add a fact to the underlying concept. For
best results a single image should be added to each and every node that appears in the
online Collections Browser. If adding an image to any term that originates from the
Webstructure list then add the image as a fact in that list. For images that appear for
terms which originate in one of the taxon group specific lists (e.g. the Vertebrates
list in the :doc:`previous example <weblist-structure>`) then you should add the fact to
the taxon group specific list within the Weblists domain (e.g. the Vertebrates list).
For the top level nodes of these lists, which are duplicated in the Webstructure list,
please add the fact to the **Webstructure** list itself, e.g. the fact for the
vertebrates image must go into the Webstructure list not the Vertebratest list. For
images associated with any species level nodes, attach the fact to the species in
whichever list in the Thesaurus contains the most up to date information for that taxon
group. 

Creating an image fact
----------------------

When adding a fact for an image, set the following options:

* **Title** - "Image"
* **Type** - "webImage"
* **Data (HTML)** - the file name of the image file
* **Language** - not used, so set to "en - English"
* **Date** - "Unknown"
* **Applies to** - "All concepts that have the same meaning"

If any of this is not clear then the *Collections* node at the top of the Webstructure 
list itself provides an example.

Where to put the image file itself
----------------------------------

The image file referred to by the fact must of course go into the correct place so that it
can appear on the website. For the image to appear correctly on the live website, place it
into ``E:\websites\drupal\sites\default\files\collections_browser`` on the SERV-DBTEST
server, or the same location on SERV-DBTEST2 for the `test version of the site
<http://testdata.mnhn.lu>`_.

.. tip::

  There is no need to provide a thumbnail version of any of these images since the website
  automatically resizes them as it needs them. So, you just need to provide a single image
  which is at least as large as the largest version of the image the website will display.
  Therefore, for best results use images which are at least 300 pixels wide.

.. todo::

  Suggest these file paths are set up as shares so that it is easy for curators to add 
  images to the hierarchy.
