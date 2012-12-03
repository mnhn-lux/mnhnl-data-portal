Adding text to nodes in the Collections Browser hierarchy
---------------------------------------------------------

Each term in the hierarchy used to populate the online Collections Browser should at least
have a description associated with it to display on the page. In addition it is possible
to optionally add a footer text to appear beneath the page, typically used to add a bit 
of supplementary information such as an interesting fact about the taxon.

.. todo::

  Add image
  
Each piece of text is added by creating a fact against a node in the Thesaurus Editor.
If adding text to any term that originates from the Webstructure list then add the text
as a fact in that list. For texts that appear for terms which originate in one of the
taxon group specific lists (e.g. the Vertebrates list in the :doc:`previous example
<weblist-structure>`) then you should add the fact to the taxon group specific list
within the Weblists domain (e.g. the Vertebrates list). For the top level nodes of these
lists, which are duplicated in the Webstructure list, please add the fact to the
**Webstructure** list itself, e.g. the fact for the vertebrates image must go into the
Webstructure list not the Vertebrates list. For texts associated with any species level
nodes, attach the fact to the species in whichever list in the Thesaurus contains the
most up to date information for that taxon group. 

To add a fact correctly which specifies text to appear in the online Collections Browser,
add a fact with the following settings:

* **Title** - whatever you like
* **Type** - "pageHeaderData"
* **Data (HTML)** - the text to display as a fact
* **Language** - set to the language you are providing for this fact. *You should provide 4
  different facts for each piece of text, one for each language.*
* **Date** - "Unknown"
* **Applies to** - "All concepts that have the same meaning"

You can add footer texts in the same way, except set the Type to pageFooterData.