*****************************************
Setup
*****************************************

If you want to build the stack from the cut project without starting it, run:

.. code:: bash

   make build

The above command will build these images:

======================= ====================================================================================
 Service                 Image name                                                                         
======================= ====================================================================================
 *jupyter*               ``sertansenturk/mlops/jupyter``  
 *mlflow*                ``sertansenturk/mlops/mlflow``   
 *postgres*              ``sertansenturk/mlops/postgres`` 
======================= ====================================================================================

.. note::

   The version tag of docker images is read from the ``VERSION`` variable in the ``.env`` file.

If you need to make a clean start:

.. code:: bash

   make clean-all
