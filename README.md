# 📝 Conversor de Arquivos – TXT / PDF / DOCX

Um utilitário em **Python 3** para conversão simples entre **TXT**, **PDF** e **DOCX** diretamente pelo terminal.  
Ideal para quem precisa transformar textos em relatórios ou documentos editáveis em poucos segundos.

---

## 🚀 Funcionalidades

- **TXT → PDF**  
- **TXT → DOCX**  
- **PDF → DOCX** (extração de texto)  
- **DOCX → PDF**

O programa é **interativo no terminal**, guiando você passo a passo para informar os caminhos de entrada e saída.

---

## 🛠️ Requisitos

- **Python 3.8+**  
- Bibliotecas Python:
  - [fpdf](https://pypi.org/project/fpdf/)  
  - [python-docx](https://pypi.org/project/python-docx/)  
  - [PyPDF2](https://pypi.org/project/PyPDF2/)

Instale tudo de uma vez:

```bash
pip install fpdf python-docx PyPDF2
```

---

## 📂 Estrutura sugerida

```
conversor/
├─ conversor.py   # Código principal
├─ exemplos/
│  ├─ teste.txt
│  └─ modelo.docx
└─ README.md
```

Você pode nomear o arquivo principal como desejar, mas aqui consideramos `conversor.py`.

---

## ▶️ Como usar

No terminal, dentro da pasta do projeto:

```bash
python conversor.py
```

Em seguida, escolha uma das opções:

```
1 - Converter de txt para PDF
2 - Converter de txt para docx
3 - Converter de PDF para docx
4 - Converter de docx para PDF
```

Depois informe:
1. O **caminho do arquivo de entrada** (por exemplo, `exemplos/teste.txt`)  
2. O **caminho de saída com extensão correta** (ex.: `saida/documento.pdf`)

---

### 🔑 Exemplo rápido

Transformar um arquivo TXT em PDF:

```bash
python conversor.py
```

Selecione: `1`  
- Caminho de entrada: `exemplos/teste.txt`  
- Caminho de saída: `saida/relatorio.pdf`

Pronto! O PDF estará em `saida/relatorio.pdf`.

---

## 💡 Observações Importantes

- Certifique-se de que os arquivos de entrada estejam **codificados em UTF-8** para evitar erros de leitura.
- Para PDF → DOCX, apenas o **texto extraído** é convertido (não preserva formatação complexa, imagens ou tabelas).
- Caso queira rodar em Windows sem digitar `python`, pode criar um atalho `.bat` chamando o script.

---

## 🏷️ Licença

Este projeto é de uso pessoal, mas você pode adaptá-lo e distribuí-lo livremente.  
Considere dar os devidos créditos se reutilizar o código.
