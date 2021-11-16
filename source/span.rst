Span
====

.. namespace:: gsl

.. class:: span

Non-member Functions
--------------------

.. function:: template <class SrcElementType, std::size_t SrcExtent, class DestElementType, std::size_t DestExtent> \
                  void copy(span<SrcElementType, SrcExtent> src, span<DestElementType, DestExtent> dest)
  :tparam-line-spec:

  Copies all the elements from one :cpp:class:`gsl::span` to another.

  According to the authors:

    This will generate faster code than `std::copy
    <https://en.cppreference.com/w/cpp/algorithm/copy>`_ using span iterator in
    older msvc+stl. [This is] not necessary for msvc since VS2017 15.8 (_MSC_VER
    >= 1915)

  :parameter src: The span to copy from.
  :parameter dest: The span to copy to.

  Preconditions
  .............
