Input & Output
==============

This section describe the format of the input and what is the output of the **sudoku** encoding.


Input
-----

.. list-table:: **Input predicate**
   :widths: 25 50 50
   :header-rows: 1

   * - Predicate
     - Arguments
     - Description
    
   * - **instance/3**
     - X → Column index of the cell

       Y → Row index of the cell

       V → Value of the cell

     - Initial value *V* of the the sudoku at cell position *(X,Y)* 


.. list-table:: **Option**
   :widths: 25 50 20
   :header-rows: 1

   * - Option name
     - Description
     - Default value

   * - **dim**
     - The dimension of the Sudoku: `dim*dim x dim*dim` grid
     - 3




Output
------

.. list-table:: **Output predicate**
   :widths: 25 50 50
   :header-rows: 1

   * - Predicate
     - Arguments
     - Description
    
   * - **sudoku/3**
     - X → Column index of the cell

       Y → Row index of the cell

       V → Value of the cell

     - Value *V* of the the sudoku at cell position *(X,Y)* 

