Contributon Documentation
=========================

*Understand the encoding*


Terms
-----

.. list-table:: **Terms definition**
   :widths: 10 30 70
   :header-rows: 1

   * - Term
     - Type
     - Description
    
   * - **X**
     - Integer 0 ≤ X ≤ 9
     - Column index of the cell

   * - **Y**
     - Integer 0 ≤ Y ≤ 9
     - Row index of the cell

   * - **V**
     - Integer 0 ≤ Y ≤ 9
     - Value of the cell



Facts
-----


.. _val1:

**val/1**
    Location: `Line;14 <https://github.com/Owrel/clindoc/blob/master/examples/sudoku_without_user_doc.lp#L14>`_

    .. literalinclude:: ../../sudoku.lp
        :language: prolog
        :linenos:
        :lines: 9


Rules
-----

**pos/2**
    Dependencies: 
         -  :ref:`val1<val/1>`
    pos(X,Y) 
         - X → Column index of the cell
         - Y → Row index of the cell

    .. literalinclude:: ../../sudoku.lp
        :language: prolog
        :linenos:
        :lines: 10

