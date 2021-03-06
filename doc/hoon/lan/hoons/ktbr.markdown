---
layout: subpage
axis: doc-hoon
categories: ket rune
sort: 52
title: ketbar
---



#[ketbar, `^|`, %ktbr](#ktbr)

##Syntax

`^|`, `ketbar`, `[%ktbr p=twig]` is a natural hoon that
converts a gold core into an iron core.

###Form

####Tall

    ^|  p

####Wide

    ^|(p)

####Irregular

    None

###Reduction

###Examples

##Semantics

###Definition

    ++  twig  
      $%  [%ktbr p=twig]
      ==

###Expansion

    ++  mint
      ?-  gen
        [%ktbr *]  =+(vat=$(gen p.gen) [(wrap(sut p.vat) %iron) q.vat])
      ==
    ++  wrap
      ~/  %wrap
      |=  yoz=?(%lead %iron %zinc)
      ^-  type
      ?-  sut
        [%core *]  ?.(=(%gold p.q.sut) ~|(%wrap-metl !!) sut(p.q yoz))
        [%fork *]  (fork $(sut p.sut) $(sut q.sut))
        [%hold *]  $(sut repo)
        *          ~|(%wrap-type !!)
      ==

##Notes

See the discussion of geometric polymorphism in chapter 10.