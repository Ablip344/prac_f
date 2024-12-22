import matplotlib.pyplot as plt
import numpy as np

# Gráficos prácticas laboratorio física

# Definir los datos para cada gráfico

# Práctica 1 - Método 1
resistencias = ['R1', 'R2', 'R3', 'R4', 'R5', 'R6']
valor_metodo1 = [10, 220000, 1000000, 22000, 22, 5600]
valor_metodo2 = [10.5, 222000, 1018000, 22000, 22.2, 5520]
diferencia = [0.5, 2000, 18000, 0, 0.2, 80]

# Práctica 1 - Método 2 (Serie y Paralelo)
req_serie_teorico = 1240000  # Resistencia equivalente teórica en serie
req_serie_practico = 1260000  # Resistencia equivalente práctica en serie
req_paralelo_teorico = 6.87  # Resistencia equivalente teórica en paralelo
req_paralelo_practico = 7.12  # Resistencia equivalente práctica en paralelo

# Práctica 2 - Proceso de carga
tiempo_carga = [2, 4, 6, 8, 10, 12, 14]
vcb_carga = [3.35, 6.35, 9, 11.5, 13.7, 15.7, 17.5]

# Práctica 2 - Proceso de descarga
tiempo_descarga = [1, 2, 3, 4, 5, 6, 7, 8, 9]
vcb_descarga = [16.4, 15.4, 14.5, 13.6, 12.8, 12.1, 11.3, 10.7, 10.05]

# Práctica 4 - Campo magnético
radio = [3, 4.24, 6, 6]
vueltas = [1, 1, 2, 3]
campo_medido = [0.1, 0.07, 0.1, 0.14]  # en mT
campo_calculado = [1.047e-4, 7.409e-5, 1.047e-4, 1.57e-4]  # en T

# Gráfico Práctica 1 - Método 1
plt.figure(figsize=(12, 8))
plt.bar(resistencias, diferencia, color='orange', alpha=0.7, label='Diferencia')
plt.title("Diferencia entre métodos (Práctica 1 - Método 1)", fontsize=14)
plt.ylabel("Diferencia (Ω)")
plt.legend()
plt.grid(True, linestyle='--', alpha=0.5)
plt.show()

# Gráfico Práctica 1 - Método 2 (Serie y Paralelo)
fig, ax = plt.subplots(1, 2, figsize=(14, 6))
ax[0].bar(['Teórico', 'Práctico'], [req_serie_teorico, req_serie_practico], color=['blue', 'green'], alpha=0.7)
ax[0].set_title("Resistencia Equivalente (Serie)")
ax[0].set_ylabel("Resistencia (Ω)")
ax[0].grid(True, linestyle='--', alpha=0.5)

ax[1].bar(['Teórico', 'Práctico'], [req_paralelo_teorico, req_paralelo_practico], color=['blue', 'green'], alpha=0.7)
ax[1].set_title("Resistencia Equivalente (Paralelo)")
ax[1].set_ylabel("Resistencia (Ω)")
ax[1].grid(True, linestyle='--', alpha=0.5)

plt.tight_layout()
plt.show()

# Gráfico Práctica 2 - Carga y Descarga
plt.figure(figsize=(12, 6))
plt.plot(tiempo_carga, vcb_carga, marker='o', label="Carga", color="blue")
plt.plot(tiempo_descarga, vcb_descarga, marker='x', label="Descarga", color="red")
plt.title("Circuito RC: Carga y Descarga", fontsize=14)
plt.xlabel("Tiempo (s)")
plt.ylabel("Voltaje (V)")
plt.legend()
plt.grid(True, linestyle='--', alpha=0.5)
plt.show()

# Gráfico Práctica 4 - Campo magnético
plt.figure(figsize=(12, 6))
plt.plot(vueltas, campo_medido, marker='o', label="Medido (mT)", color="green")
plt.plot(vueltas, campo_calculado, marker='x', label="Calculado (T)", color="purple")
plt.title("Campo Magnético vs. Número de Vueltas (Práctica 4)", fontsize=14)
plt.xlabel("Número de Vueltas")
plt.ylabel("Campo Magnético")
plt.legend()
plt.grid(True, linestyle='--', alpha=0.5)
plt.show()
