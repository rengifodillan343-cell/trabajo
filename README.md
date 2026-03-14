# trabajo
# solicitar nombre del producto
producto = input("Ingrese el nombre del producto: ")

# validar que el precio sea un número decimal positivo
while True:
    try:
        precio_producto = float(input("Ingrese el precio del producto: "))
        if precio_producto <= 0:
            print("El precio debe ser mayor que 0.\n")
            continue
        break
    except ValueError:
        print("Entrada inválida. Intente otra vez.\n")

# validar que la cantidad sea un número entero positivo
while True:
    try:
        cantidad_producto = int(input("Ingrese la cantidad: "))
        if cantidad_producto <= 0:
            print("La cantidad debe ser mayor que 0.\n")
            continue
        break
    except ValueError:
        print("Debe ingresar un número entero.\n")

# cálculo del costo total
total = precio_producto * cantidad_producto

# mostrar resultado final
print(f"\nProducto: {producto}")
print(f"Precio unitario: {precio_producto}")
print(f"Cantidad: {cantidad_producto}")
print(f"Costo total: {total}")

