---
layout: subpage
axis: doc-hoon
categories: buc rune
sort: 2
title: buccol
---

#buccol `$:` %bccl

##Syntax

`$:`, `buccol`, is a tile hoon that declares a tile autocons,`[p=tile q=tile]`.

###Form
`p` is a tile
`q` is a tile

####Tall

    $:  p
        q
    ==

####Wide

    $:(p q)

####Irregular

    [p q]

###Reduction
None

##Semantics

`$:` is tile.

###Definition###

    ++  tile  $&  [p=tile q=tile]                           ::  ordered pair

###Expansion
None


###Notes###

Tiles autocons, just like twigs - a cell of tiles is a tile of a cell. But we shouldn't skip the differences too lightly.

A cell of twigs is also a twig of a cell. But in the cell of twigs, the subject of either leg is the original subject. Whereas when applying a tile in a whip or clam, the subject is split in half for equally obvious reasons.

(Otherwise, how would `(,[@ @] [4 5])` be `[4 5]`? Clearly, this should be the same as `[(,@ 4) (,@ 5)]`. Clearly, it should not be the same as `[(,@ [4 5]) (,@ [4 5])]` - which would produce merely `[0 0]`.)


