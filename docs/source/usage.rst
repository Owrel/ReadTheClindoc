Usage
=====

.. _installation:

Installation
------------

To use the sudoku solver, clone the git repo:

.. code-block:: console

   git clone https://github.com/Owrel/ReadTheClindoc.git

Solving an instance
-------------------

To solve an instance, we use the ASP solver `clingo <https://potassco.org/clingo/>`_. With the following commandline :

.. code-block:: console

   clingo sudoku.lp instance.lp 1

Where `instance.lp` is a file containing a valid input instance


Example
-------

instance (as *instance.lp*):

.. code-block:: cplint

   instance(2,3,7). instance(3,3,6). instance(4,3,5). instance(5,3,1).
   instance(6,3,8). instance(7,3,3). instance(8,3,2). instance(9,3,4).
   instance(1,4,3). instance(2,4,6). instance(3,4,2). instance(4,4,4).
   instance(5,4,8). instance(6,4,5). instance(7,4,1). instance(8,4,9).
   instance(9,4,7). instance(1,5,4). instance(2,5,1). instance(3,5,5).
   instance(4,5,9). instance(5,5,6). instance(6,5,7). instance(7,5,8).
   instance(8,5,3). instance(9,5,2). instance(1,6,8). instance(2,6,9).
   instance(3,6,7). instance(4,6,1). instance(5,6,3). instance(6,6,2).
   instance(7,6,4). instance(8,6,5). instance(9,6,6). instance(1,7,5).
   instance(2,7,8). instance(3,7,1). instance(4,7,6). instance(5,7,4).
   instance(6,7,3).


Command line:

.. code-block:: console

   clingo sudoku.lp instance.lp 1


Output:

.. code-block:: cplint

   sudoku(2,3,7) sudoku(3,3,6) sudoku(4,3,5) sudoku(5,3,1) 
   sudoku(6,3,8) sudoku(7,3,3) sudoku(8,3,2) sudoku(9,3,4) 
   sudoku(1,4,3) sudoku(2,4,6) sudoku(3,4,2) sudoku(4,4,4) 
   sudoku(5,4,8) sudoku(6,4,5) sudoku(7,4,1) sudoku(8,4,9) 
   sudoku(9,4,7) sudoku(1,5,4) sudoku(2,5,1) sudoku(3,5,5) 
   sudoku(4,5,9) sudoku(5,5,6) sudoku(6,5,7) sudoku(7,5,8) 
   sudoku(8,5,3) sudoku(9,5,2) sudoku(1,6,8) sudoku(2,6,9) 
   sudoku(3,6,7) sudoku(4,6,1) sudoku(5,6,3) sudoku(6,6,2) 
   sudoku(7,6,4) sudoku(8,6,5) sudoku(9,6,6) sudoku(1,7,5) 
   sudoku(2,7,8) sudoku(3,7,1) sudoku(4,7,6) sudoku(5,7,4) 
   sudoku(6,7,3) sudoku(1,1,1) sudoku(2,1,4) sudoku(3,1,3) 
   sudoku(4,1,7) sudoku(5,1,2) sudoku(6,1,6) sudoku(7,1,9) 
   sudoku(8,1,8) sudoku(9,1,5) sudoku(1,2,2) sudoku(2,2,5) 
   sudoku(3,2,8) sudoku(4,2,3) sudoku(5,2,9) sudoku(6,2,4) 
   sudoku(7,2,7) sudoku(8,2,6) sudoku(9,2,1) sudoku(1,3,9) 
   sudoku(7,7,2) sudoku(8,7,7) sudoku(9,7,9) sudoku(1,8,7) 
   sudoku(2,8,3) sudoku(3,8,9) sudoku(4,8,2) sudoku(5,8,5) 
   sudoku(6,8,1) sudoku(7,8,6) sudoku(8,8,4) sudoku(9,8,8) 
   sudoku(1,9,6) sudoku(2,9,2) sudoku(3,9,4) sudoku(4,9,8) 
   sudoku(5,9,7) sudoku(6,9,9) sudoku(7,9,5) sudoku(8,9,1) 
   sudoku(9,9,3)