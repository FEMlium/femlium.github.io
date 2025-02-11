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

Installation and usage
----------------------

Simply clone the **FEMlium** public repository:

.. code-block:: console

    git clone https://github.com/FEMlium/FEMlium.git

and install the package by typing

.. code-block:: console

    cd FEMlium
    python3 -m pip install '.[tutorials]'

Compatibility with upstream releases
------------------------------------

The :code:`main` branch of **FEMlium** targets the :code:`main` branch of :code:`dolfinx` and :code:`firedrake`, which may contain API changes compared to the latest release of the finite element backend. A new **FEMlium** version is not necessarily tagged alongside :code:`dolfinx` or :code:`firedrake` releases. Users willing to work with a fixed release of the finite element backend are encouraged to look for a **FEMlium** `commit <https://github.com/FEMlium/FEMlium/commits/main>`__ close to the upstream release date, and do a

.. code-block:: console

    git checkout {commit SHA}

before installing **FEMlium**.
