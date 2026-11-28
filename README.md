# Organizador de Arquivos

Script em Python que organiza automaticamente os arquivos de uma pasta em subpastas por categoria, com base na extensão de cada arquivo, evitando sobrescrever arquivos já existentes.

## Instalação

1. Certifique-se de ter o **Python 3.8+** instalado.
2. Clone o repositório:
   ```bash
   git clone [https://github.com/guilhermetorres-RedesComp/Atividade_git13.git](https://github.com/guilhermetorres-RedesComp/Atividade_git13.git)
   cd Atividade_git13
   ```

## Uso

Importe a função `organize_folder` do arquivo `organizer.py` informando a pasta alvo e o mapa de extensões:

```python
from pathlib import Path
from organizer import organize_folder

extensoes = {
    "Imagens": [".jpg", ".jpeg", ".png", ".gif"],
    "Documentos": [".pdf", ".docx", ".txt"],
    "Planilhas": [".xlsx", ".csv"],
}

organize_folder(Path("./Downloads"), extensoes)
```

Arquivos cuja extensão não estiver mapeada são movidos automaticamente para a pasta `Outros`.

## Licença

Este projeto está sob a licença MIT.
