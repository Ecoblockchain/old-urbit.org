---
layout: subpage
title: Tiles
axis: doc-hoon
categories: lan overview
sort: 3
---

    ++  tile  $&  [p=tile q=tile]                           ::  ordered pair
              $%  [%axil p=base]                            ::  base type
                  [%bark p=term q=tile]                     ::  name
                  [%bush p=tile q=tile]                     ::  pair/tag
                  [%fern p=[i=tile t=(list tile)]]          ::  plain selection
                  [%herb p=twig]                            ::  function
                  [%kelp p=[i=line t=(list line)]]          ::  tag selection
                  [%leaf p=term q=@]                        ::  constant atom
                  [%reed p=tile q=tile]                     ::  atom/cell
                  [%weed p=twig]                            ::  example
              ==  




    @c              UTF-32 codepoint
    @d              date
      @da           absolute date
      @dr           relative date (ie, timespan)
    @f              yes or no (inverse boolean)
    @n              nil
    @p              phonemic base
    @r              IEEE floating-point
      @rd           double precision  (64 bits)
      @rh           half precision (16 bits)
      @rq           quad precision (128 bits)
      @rs           single precision (32 bits)
    @s              signed integer, sign bit low
      @sb           signed binary
      @sd           signed decimal
      @sv           signed base32
      @sw           signed base64
      @sx           signed hexadecimal
    @t              UTF-8 text (cord)
      @ta           ASCII text (span)
        @tas        ASCII symbol (term)
    @u              unsigned integer
      @ub           unsigned binary
      @ud           unsigned decimal
      @uv           unsigned base32
      @uw           unsigned base64
      @ux           unsigned hexadecimal


#Size:
    A   1 bit
    B   2 bits
    C   4 bits
    D   1 byte
    E   2 bytes
    F   4 bytes
    G   8 bytes
    H   16 bytes
    I   32 bytes
    J   64 bytes
    K   128 bytes
    L   256 bytes
    M   512 bytes
    N   1K
    O   2K
    P   4K
    Q   8K
    R   16K
    S   32K
    T   64K
    U   128K
    V   256K
    W   512K
    X   1MB
    Y   2MB
    Z   4MB