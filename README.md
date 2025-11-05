# Gerador de Relatórios PDF com Threads

Este projeto gera relatórios em PDF a partir de dados de um arquivo CSV, utilizando múltiplas threads para acelerar o processo. Cada PDF contém até 10 registros do CSV.

## Funcionalidades

- Geração automática de arquivo CSV de exemplo (`gerar_csv.py`)
- Leitura de dados do CSV e divisão em partes
- Criação de múltiplos arquivos PDF em paralelo (usando threads)
- Testes automatizados com pytest

## Estrutura

```
data/dados.csv         # Arquivo de dados de entrada
output/                # PDFs gerados
main.py                # Script principal
gerar_csv.py           # Gera dados de exemplo
requirements.txt       # Dependências
tests/                 # Testes automatizados
```

## Como usar

1. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

2. Gere o arquivo CSV de exemplo:
   ```bash
   python gerar_csv.py
   ```

3. Execute o gerador de PDFs:
   ```bash
   python main.py
   ```

Os arquivos PDF serão criados na pasta `output/`.

## Testes

Para rodar os testes:
```bash
pytest
```

## Dependências

- Python 3.8+
- fpdf
- pytest

---
