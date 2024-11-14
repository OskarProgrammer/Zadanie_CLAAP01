
Przykład zastosowania klasy do implementacji stosu
==================================================

Najpierw deklarujemy klase
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

    class Stos(object):
        pass


Nastepnie implementujemy metodę dodawania do stosu
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

    class Stos(object):
        __data = []

        def dodajDoStosu(self , data : int ):

            self.__data.append(data)
            print(f"${data} zostala dodana do stosu!")


Należy również zaimplementować metodę zdejmowania ze stosu
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

    class Stos(object):
        __data = []

        def dodajDoStosu(self , data : int ):

            self.__data.append(data)
            print(f"${data} zostala dodana do stosu!")

        def zdejmijZeStosu(self) -> int:

            if (len(self.__data) == 0 ) : 
                return -1

            toReturn = self.__data[-1]
            del self.__data[-1]

            return toReturn


Przydałaby się metoda czyszcząca nasz stos
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

    class Stos(object):
        __data = []

        def dodajDoStosu(self , data : int ):

            self.__data.append(data)
            print(f"${data} zostala dodana do stosu!")

        def zdejmijZeStosu(self) -> int:

            if (len(self.__data) == 0 ) : 
                return -1

            toReturn = self.__data[-1]
            del self.__data[-1]

            return toReturn
        
        def czyscStos(self) : 

            self.__data = []
            print(f"Stos wyczyszczony")



Zaimplementujemy metodę, która zostanie wywołana przy `len(obiekt)`
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

    class Stos(object):
        __data = []

        def dodajDoStosu(self , data : int ):

            self.__data.append(data)
            print(f"${data} zostala dodana do stosu!")

        def zdejmijZeStosu(self) -> int:

            if (len(self.__data) == 0 ) : 
                return -1
                
            toReturn = self.__data[-1]
            del self.__data[-1]

            return toReturn
        
        def czyscStos(self) : 

            self.__data = []
            print(f"Stos wyczyszczony")
        
        def __len__(self) -> int:

            return len(self.__data)




    