
Metody Magiczne Klas
====================

.. py:method:: __init__(self, ...)

    Jest wywoływana przy każdej inicjalizacji nowej instancji klasy

.. py:method:: __del__(self, ...)
    
    Jest wywoływana przy każdym usunięciu instancji klasy

.. py:method:: __repr__(self, ...)

    Jest wywoływana przy każdym wywołaniu obiektu samego w sobie, zwykle powinna zwracać reprezentację tekstową obiektu

.. py:method:: __hash__(self)

    Jest wykorzystywana do haszowania obiektu, czyli podczas zamiany na reprezentacje liczbową

.. py:method:: __str__(self)

    Jest wywoływana przy każdej konwersji *obiektu* do łańcucha znaków tzn.

.. code-block:: python

        str(obiekt)

.. py:method:: __int__(self)

    Jest wywoływana przy każdej konwersji *obiektu* do liczby całkowitoliczbowejn tzn.

.. code-block:: python

        int(obiekt)

.. py:method:: __float__(self)

    Jest wywoływana przy każdej konwersji *obiektu* do liczby zmiennoprzecinkowej tzn.

.. code-block:: python

        float(obiekt)

.. py:method:: __len__(self)

    Jest wywoływana przy każdym wywołaniu na *obiekcie* len tzn.

.. code-block:: python

        len(obiekt)

