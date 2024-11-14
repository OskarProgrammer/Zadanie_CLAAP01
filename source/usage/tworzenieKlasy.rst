

Początek przygody z klasami w python
====================================


Deklarowanie klasy
------------------

.. code-block:: python
    
    class NazwaKlasy(object):
        pass


Tworzenie metod klasy
---------------------

Metody publiczne
^^^^^^^^^^^^^^^^

.. code-block:: python

    class NazwaKlasy(object):
        def nazwaMetody(self):
            pass

Metody prywatne
^^^^^^^^^^^^^^^^

.. code-block:: python

    class NazwaKlasy(object):
        def __nazwaMetody(self):
            pass

Metody chronione
^^^^^^^^^^^^^^^^

.. code-block:: python

    class NazwaKlasy(object):
        def _nazwaMetody(self):
            pass

Tworzenie pól klasy
---------------------

Pola publiczne
^^^^^^^^^^^^^^^^

.. code-block:: python

    class NazwaKlasy(object):
        def __init__(self):
            polePubliczne = 2

Pola prywatne
^^^^^^^^^^^^^^^^

.. code-block:: python

    class NazwaKlasy(object):
        def __init__(self):
            __polePrywatne = 2

Pola chronione
^^^^^^^^^^^^^^^^

.. code-block:: python

    class NazwaKlasy(object):
        def __init__(self):
            _polePrywatne = 2


Inicjalizowanie obiektu klasy
-----------------------------

.. code-block:: python

    obiekt = NazwaKlasy()


Wywolywanie metody na obiekcie klasy
------------------------------------

.. code-block:: python

    obiekt = NazwaKlasy()
    obiekt.nazwaMetody()