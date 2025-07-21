Installation
============
.. meta::
    :description lang=en:
        FEMlium is available on PyPI. Use pip extras to install all required dependencies.
        In order to run the tutorials you may need to install one of the supported finite element backends.

Prerequisites
-------------

In order to run the tutorials you may need to install one of the supported finite element backends, namely `dolfinx <https://github.com/FEniCS/dolfinx>`__ and `firedrake <https://github.com/firedrakeproject/firedrake>`__.

Installation
------------

**FEMlium** is available on PyPI. Use `pip` extras to select the finite element backend and install additional dependencies needed for the tutorials.

Installation with the dolfinx backend
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: console

    python3 -m pip install 'femlium[backend-dolfinx,tutorials]'

Installation with the firedrake backend
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: console

    python3 -m pip install 'femlium[backend-firedrake,tutorials]'

Running tutorials
-----------------

To run the tutorials, first clone the **FEMlium** repository. Then, ensure you check out the tag that corresponds to the version of **FEMlium** currently installed.

.. code-block:: console

    git clone https://github.com/FEMlium/FEMlium.git
    cd femlium
    FEMLIUM_VERSION=$(python3 -c "import femlium; print(femlium.__version__)")
    git checkout ${FEMLIUM_VERSION}
