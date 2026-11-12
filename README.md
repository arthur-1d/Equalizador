# AudioLab — Equalizador de som com Arduino

Site educativo feito com **Python + Flask**, HTML e CSS. O conteúdo apresenta o funcionamento de um equalizador convencional e documenta o protótipo escolar com Arduino UNO, sensor KY-038, protoboard e LEDs, incluindo a falha de mau contato relatada na montagem.

## Como executar no VS Code

1. Instale o Python 3.
2. Abra esta pasta no VS Code.
3. No terminal, crie um ambiente virtual (opcional, mas recomendado):

   ```bash
   python -m venv .venv
   ```

4. Ative o ambiente virtual:

   **Windows PowerShell**
   ```powershell
   .venv\Scripts\Activate.ps1
   ```

   **Windows CMD**
   ```cmd
   .venv\Scripts\activate
   ```

5. Instale as dependências:

   ```bash
   pip install -r requirements.txt
   ```

6. Inicie o site:

   ```bash
   python app.py
   ```

7. Abra no navegador o endereço indicado no terminal, normalmente `http://127.0.0.1:5000`.

## Publicar no GitHub

Envie a pasta do projeto para um repositório GitHub. O GitHub Pages não executa aplicações Flask/Python diretamente: ele hospeda sites estáticos. Para manter o Flask, publique a aplicação em uma plataforma que execute Python (por exemplo, Render) e use o GitHub para armazenar o código.

## Estrutura

```text
equalizador_arduino_site/
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
├── templates/
│   └── index.html
└── static/
    └── css/
        └── style.css
```

## Nota técnica

O KY-038 é um módulo de detecção de som com microfone e saídas analógica/digital. Ele pode ser usado para reagir à intensidade sonora, mas não separa por si só o áudio em graves, médios e agudos. Por isso, o site descreve a montagem como um indicador luminoso de som, diferenciando-a de um equalizador de frequência completo.
