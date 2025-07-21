Installation
============
.. meta::
    :description lang=en:
        Installation requirements are automatically handled during the setup.
        In order to run the tutorials you may need to install one of the supported finite element backends.

Prerequisites
-------------

Installation requirements are automatically handled during the setup.
In order to run the tutorials you may need to install one of the supported finite element backends, namely `dolfinx <https://github.com/FEniCS/dolfinx>`__ and `firedrake <https://github.com/firedrakeproject/firedrake>`__.

Installation
------------

**FEMlium** is available on PyPI. It uses extras to specify the finite element backend when installing via `pip` and to install additional packages required to run the tutorials.

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
