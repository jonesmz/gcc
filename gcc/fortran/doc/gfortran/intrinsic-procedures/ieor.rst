..
  Copyright 1988-2022 Free Software Foundation, Inc.
  This is part of the GCC manual.
  For copying conditions, see the copyright.rst file.

.. _ieor:

.. index:: IEOR

.. index:: BIEOR

.. index:: IIEOR

.. index:: JIEOR

.. index:: KIEOR

.. index:: bitwise logical exclusive or

.. index:: logical exclusive or, bitwise

IEOR --- Bitwise logical exclusive or
*************************************

.. function:: IEOR()

  ``IEOR`` returns the bitwise Boolean exclusive-OR of :samp:`{I}` and
  :samp:`{J}`.

  :param I:
    The type shall be ``INTEGER`` or a boz-literal-constant.

  :param J:
    The type shall be ``INTEGER`` with the same
    kind type parameter as :samp:`{I}` or a boz-literal-constant.
    :samp:`{I}` and :samp:`{J}` shall not both be boz-literal-constants.

  :return:
    The return type is ``INTEGER`` with the kind type parameter of the
    arguments.
    A boz-literal-constant is converted to an ``INTEGER`` with the kind
    type parameter of the other argument as-if a call to :ref:`INT` occurred.

  Standard:
    Fortran 90 and later, with boz-literal-constant Fortran 2008 and later, has overloads that are GNU extensions

  Class:
    Elemental function

  Syntax:
    .. code-block:: fortran

      RESULT = IEOR(I, J)

  Specific names:
    .. list-table::
       :header-rows: 1

       * - Name
         - Argument
         - Return type
         - Standard

       * - ``IEOR(A)``
         - ``INTEGER A``
         - ``INTEGER``
         - Fortran 90 and later
       * - ``BIEOR(A)``
         - ``INTEGER(1) A``
         - ``INTEGER(1)``
         - GNU extension
       * - ``IIEOR(A)``
         - ``INTEGER(2) A``
         - ``INTEGER(2)``
         - GNU extension
       * - ``JIEOR(A)``
         - ``INTEGER(4) A``
         - ``INTEGER(4)``
         - GNU extension
       * - ``KIEOR(A)``
         - ``INTEGER(8) A``
         - ``INTEGER(8)``
         - GNU extension

  See also:
    :ref:`IOR`,
    :ref:`IAND`,
    :ref:`IBITS`,
    :ref:`IBSET`,
    :ref:`IBCLR`,
    :ref:`NOT`
