---
layout: subpage
axis: doc-hoon
categories: hax rune
sort: 50
title: haxgal
---



#[haxgal, `#<`, %hxgl](#hxgl)

##Syntax

`#<`, `haxgal`, `[%hxgl p=tusk]`is a synthetic hoon that
slams the assumed gate `noah` on `[%zpgr %cntr p]`.

###Form

####Tall

    ?

####Wide

    ?

####Irregular

    >i.p i.t.p i.t.t.p<

###Reduction

###Examples

##Semantics

###Definition

    ++  twig  
      $%  [%hxgl p=tusk]
      ==
++  tusk  (list twig)

###Expansion

    ++  open
      ^-  twig
      ?-  gen
        [%hxgl *]
      [%cnhp [%cnzy %noah] [%zpgr [%cltr p.gen]] ~]
      ==

##Notes

`noah` is one of four "Biblical" names that the Hoon compiler, violating its usual principles, generates automatically.

Of course the compiler cannot control what `noah` produces when pulled from the subject, but the convention is that it should be a gate that accepts a `vase` (type-value cell) and produces a `tank` (pretty-printer input).