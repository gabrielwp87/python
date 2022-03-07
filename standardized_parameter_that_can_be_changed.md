In a function it is possible to stadarize a parameter, so when the function doesn't receive it's parameter it will use the already set as it's standard.

E.g.
class Conta:

    def __init__(self, numero, titular, saldo, limite = 1000.0):
        self.numero = numero
        self.titular = titular
        self.saldo = saldo
        self.limite = limite
        
        conta1 = Conta(1, "Fulano", 0.0)
        conta2 = Conta(2, "Beltrano", 0.0)
        conta3 = Conta(3, "Sicrano", 0.0, 2000.0)
       
In this case conta1 and conta2 will have a limite of 1000.0.
