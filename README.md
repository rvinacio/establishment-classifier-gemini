## establishment-classifier-gemini

Este repositório apresenta um script Python que utiliza o poder do modelo de linguagem Gemini da Google para automatizar a categorização de estabelecimentos comerciais com base em seus nomes.

## Descrição

O script analisa os nomes de estabelecimentos fornecidos como entrada e os classifica em categorias relevantes, como "Saúde", "Alimentação", "Transporte", etc. Além da categoria, o script também fornece uma breve justificativa para cada classificação, auxiliando na compreensão da decisão do modelo.

## Funcionalidades

* **Categorização Inteligente:** Utiliza o modelo Gemini da Google, treinado em uma vasta quantidade de dados, para classificar estabelecimentos com precisão.
* **Justificativas Detalhadas:** Explica por que cada estabelecimento foi classificado em determinada categoria, aumentando a transparência e a confiança nos resultados.
* **Interface Simples:** A interação com o script é fácil e intuitiva. Basta inserir os nomes dos estabelecimentos separados por vírgula.
* **Tratamento de Erros e Formatos Inesperados:** O script lida com respostas do modelo que não seguem o formato padrão e com inconsistências nos dados de entrada, garantindo a robustez da solução.
* **Customização:** O código é facilmente adaptável para diferentes modelos de linguagem da Google ou para cenários de classificação mais específicos.

## Como Usar

1. **Clone o Repositório:**

   ```bash
   git clone https://github.com/seu-usuario/establishment-classifier-gemini.git
   ```

2. **Instale as Dependências:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Configure sua Chave de API:**

   * Obtenha uma chave de API do Google Cloud Console.
   * Crie um arquivo `credentials.json` na raiz do projeto e insira sua chave.

4. **Execute o Script:**

   ```bash
   python main.py
   ```

5. **Insira os Estabelecimentos:**

   * Digite os nomes dos estabelecimentos separados por vírgula e pressione Enter.

## Exemplo

```
Digite os nomes dos estabelecimentos (separados por vírgula): Padaria do Zé, Clínica Saúde & Vida, Restaurante Sabor da Terra
input: Padaria do Zé
output: Alimentação
output_justificativa: Padaria

input: Clínica Saúde & Vida
output: Saúde
output_justificativa: Clínica

input: Restaurante Sabor da Terra
output: Alimentação
output_justificativa: Restaurante
```

## Tecnologias Utilizadas

* Python
* Google Generative AI
* Google Gemini

## Contribuição

Sinta-se à vontade para contribuir com melhorias, correções ou novos recursos!

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
