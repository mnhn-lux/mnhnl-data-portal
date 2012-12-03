Structure of the Collections Browser hierarchy
==============================================

The Collections Browser uses a hierarchy that is derived from lists in the Thesaurus
Editor to provide a means of browsing through the specimens in the collections. Rather
than use a single list, each branch of taxonomy within the hierarchy has its own list
which allows curators to be responsible for their own parts of the hierarchy. All the
lists involved belong to the **Weblists** domain, in the **General Term Lists** section
of the Thesaurus. At the very top of the hierarchy a list called **Webstructure**
provides the first few levels of the browsing hierarchy, down to the point where the
hierarchy splits into taxonomic divisions appropriate for allocation to different
curators. 

As well as the Webstructure list there are then additional taxon group specific lists in
the Weblists domain, each of which has a top-level node that exactly matches a bottom
level node in the Webstructure list. This allows the lists to be "joined" together to
make a single hierarchy. These taxon group specific lists only need to go down as many
levels as the curator feels appropriate until the point where the list of species below
the bottom level is manageable for browsing. For example, if their are many genera and
species within a family, it might be appropriate to define a hierarchy in the group
specific list that goes right down to genus level, so the user attempting to find a
species needs only to look through the species in a single genus. On the other hand if
there are only a few taxa in a family it might be appropriate to only go down as far as
family level so the user sees all species in the family on a single browsing page. Note 
that the website will automatically show all species below whatever the bottom level is
in the list so there is no need to add the species to the hierarchy. 

To illustrate this, consider the following hierarchy which the user might browse through ::

  Collections > Zoology Collections > Vertebrates > Birds > Columbiformes > Columba palumbus

The Webstructure list might contain the following levels::

  Collections > Zoology Collections > Vertebrates
  
Then, there should be a list called Vertebrates which is managed by the curator of 
vertebrates in the museum. This list contains the following term hierarchy:: 

  Vertebrates > Birds > Columbiformes
  
The Columbiformes term must be linked to the rest of the thesaurus lists in order to
determine which species it contains. It doesn't matter if the other nodes in the
hierarchy are not linked as synonyms with the equivalent terms in other lists. The term
for **Columba palumbus**, along with all the other Columbiforme species which the museum
hold specimens for, is then automatically included in the hierarchy because it can be
determined as a child of Columbiformes via one of the other lists.

.. note::

  The curator in this instance could opt to add a term for Columba beneath Columbiformes
  if they want the user to browse right down to genus level, in which case they must 
  ensure that the Columba term is linked correctly to the rest of the Thesaurus.

