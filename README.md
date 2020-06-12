# Resto Apertura Comandas (Mostrador y Delivery)

La API permite registrar en la base de datos de Tango Restó, las comandas o pedidos generados por aplicaciones externas. Esta información es recibida como parámetros de entrada y la comanda será visualiza en el módulo de Delivery o Mostrador según sea el caso.

Desde Restô se podrá:
  - Identificar el origen de la comanda. 
  - Cancelar una comanda.
  - Crear un cliente si no existe siendo la dirección de entrega la que indique un método para agregar una comanda.


## Arquitectura

![imagenapi](https://github.com/TangoSoftware/RestoAperturaComandasMostradorDelivery/blob/master/00.jpg)

## Métodos

### 1. AddOrder (POS)
  Este método permite registrar una nueva orden de pedido en la base de datos del sistema Tango Restó

####   Request
     - TokenCS
     - CashCode
