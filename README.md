# 📉 Calculadora de Desconto em Python com pytest

Este projeto implementa uma função em **Python** para calcular o preço final de um produto após aplicar um desconto percentual.
O projeto também inclui **testes automatizados utilizando Pytest** para garantir o funcionamento correto da função.

---

## 📌 Funcionalidades

* Calcula o preço final após aplicar um desconto percentual.
* Valida valores de entrada:

  * O preço não pode ser negativo.
  * A porcentagem deve estar entre **0 e 100**.
* Retorna o valor final **arredondado para duas casas decimais**.
* Inclui **testes automatizados com Pytest**.

---

## 🧠 Lógica do cálculo

A fórmula utilizada é:

```python
preco_final = preco * (1 - porcentagem / 100)
```

Exemplo:

| Preço | Desconto | Resultado |
| ----- | -------- | --------- |
| 200   | 10%      | 180       |
| 150   | 100%     | 0         |
| 99.99 | 15%      | 84.99     |

---

## 📂 Estrutura do Projeto

```
project/
│
├── src/
│   └── calcular/
│       └── desconto.py
│
├── tests/
│   └── test_desconto.py
│
└── README.md
```

---

## ⚙️ Instalação

Clone o repositório:

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```

Entre na pasta do projeto:

```bash
cd seu-repositorio
```

Instale as dependências:

```bash
pip install pytest
```

---

## ▶️ Executando os testes

Para rodar os testes automatizados:

```bash
pytest
```

Se tudo estiver correto, você verá algo parecido com:

```
8 passed in 0.05s
```

---

## 📌 Exemplo de uso

```python
from src.calcular.desconto import calcular_desconto

preco = 200
desconto = 10

resultado = calcular_desconto(preco, desconto)

print(resultado)
```

Saída esperada:

```
180.0
```

---

## 🧪 Cenários testados

Os testes cobrem:

### Casos válidos

* Desconto 0%
* Desconto parcial
* Desconto 100%
* Preço 0
* Diferentes valores decimais

### Casos inválidos

* Preço negativo
* Porcentagem negativa
* Porcentagem maior que 100

---

## 🛠 Tecnologias utilizadas

* Python
* Pytest

---

## 📜 Licença

Este projeto foi desenvolvido por Mel Leticia, para fins educacionais.
