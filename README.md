# Simulações de Física

## Estrutura do Projeto

# 📂 simulacoes_fisica/
# ├── 📁 codigo_python/         # Scripts em Python
# │   ├── mru.py               # Simulação de MRU
# │   ├── forca_resultante.py  # Simulação de força resultante
# │   ├── ondas.py             # Simulação de ondas
# │   └── termodinamica.py     # Simulação de leis da termodinâmica
# ├── 📁 codigo_js/            # Simulações interativas em JavaScript
# ├── 📁 docs/                 # Documentação e explicações teóricas
# ├── README.md                # Apresentação do projeto

# Exemplo de código Python para MRU
import numpy as np
import matplotlib.pyplot as plt

def mru(velocidade, tempo):
    """Simula um Movimento Retilíneo Uniforme (MRU)"""
    t = np.linspace(0, tempo, num=100)
    x = velocidade * t
    
    plt.plot(t, x, label=f'v={velocidade} m/s')
    plt.xlabel('Tempo (s)')
    plt.ylabel('Posição (m)')
    plt.title('Movimento Retilíneo Uniforme')
    plt.legend()
    plt.grid()
    plt.show()

# Exemplo de uso
tempo_total = 10  # segundos
velocidade_mru = 5  # m/s
mru(velocidade_mru, tempo_total)

