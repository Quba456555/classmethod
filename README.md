# classmethod
import math

class WzoryMatematyczne:
    @classmethod
    def dodawanie(cls, a, b):
        return a + b

    @classmethod
    def odejmowanie(cls, a, b):
        return a - b

    @classmethod
    def mnozenie(cls, a, b):
        return a * b

    @classmethod
    def dzielenie(cls, a, b):
        if b != 0:
            return a / b
        else:
            return "Nie można dzielić przez zero."

    @classmethod
    def potegowanie(cls, a, b):
        return a ** b

    @classmethod
    def pierwiastek_kwadratowy(cls, a):
        return math.sqrt(a)

    @classmethod
    def sin(cls, a):
        return math.sin(a)

    @classmethod
    def cos(cls, a):
        return math.cos(a)

    @classmethod
    def tangens(cls, a):
        return math.tan(a)

    @classmethod
    def logarytm(cls, a):
        if a > 0:
            return math.log(a)
        else:
            return "Logarytm z liczby mniejszej lub równej zeru nie istnieje."

    @classmethod
    def silnia(cls, a):
        return math.factorial(a)

    @classmethod
    def kombinacja(cls, a, b):
        return math.comb(a, b)

    @classmethod
    def najwiekszy_wspolny_dzielnik(cls, a, b):
        return math.gcd(a, b)

    @classmethod
    def liczba_pi(cls):
        return math.pi

    @classmethod
    def liczba_e(cls):
        return math.e

if __name__ == "__main__":
    # Tworzymy instancję klasy PrzeliczWzoryMatematyczne bez konstruktora
    obiekt_matematyka = WzoryMatematyczne()

    # Przykładowe wywołanie metod na obiekcie, przekazując argumenty
    print("Dodawanie:", obiekt_matematyka.dodawanie(4, 2))
    print("Odejmowanie:", obiekt_matematyka.odejmowanie(4, 2))
    print("Mnożenie:", obiekt_matematyka.mnozenie(4, 2))
    print("Dzielenie:", obiekt_matematyka.dzielenie(4, 2))
    print("Potęgowanie:", obiekt_matematyka.potegowanie(2, 3))
    print("Pierwiastek kwadratowy:", obiekt_matematyka.pierwiastek_kwadratowy(9))
    print("Sinus:", obiekt_matematyka.sin(math.pi / 2))
    print("Cosinus:", obiekt_matematyka.cos(0))
    print("Tangens:", obiekt_matematyka.tangens(math.pi / 4))
    print("Logarytm:", obiekt_matematyka.logarytm(10))
    print("Silnia:", obiekt_matematyka.silnia(5))
    print("Kombinacja:", obiekt_matematyka.kombinacja(5, 2))
    print("Największy wspólny dzielnik:", obiekt_matematyka.najwiekszy_wspolny_dzielnik(24, 36))
    print("Liczba Pi:", obiekt_matematyka.liczba_pi())
    print("Liczba e:", obiekt_matematyka.liczba_e())
