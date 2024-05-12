## establishment-classifier-gemini

Este repositório contém um script Python que utiliza o modelo de linguagem Gemini da Google para automatizar a categorização de estabelecimentos comerciais a partir de seus nomes. Essa ferramenta é especialmente útil para **analisar gastos em extratos de cartão de crédito**, permitindo identificar padrões de consumo e otimizar o orçamento pessoal.

### Descrição

O script analisa os nomes dos estabelecimentos presentes no extrato e os classifica em categorias relevantes, como "Saúde", "Alimentação", "Transporte", etc. Além da categoria, o script também fornece uma breve justificativa para cada classificação, auxiliando na compreensão da decisão do modelo e na análise dos gastos.

### Funcionalidades

* **Categorização Inteligente:** Utiliza o modelo Gemini da Google, treinado em uma vasta quantidade de dados, para classificar estabelecimentos com precisão.
* **Justificativas Detalhadas:** Explica por que cada estabelecimento foi classificado em determinada categoria, aumentando a transparência e a confiança nos resultados.
* **Interface Simples:** A interação com o script é fácil e intuitiva, bastando inserir os nomes dos estabelecimentos separados por vírgula.
* **Tratamento de Erros e Formatos Inesperados:** O script lida com respostas do modelo que não seguem o formato padrão e com inconsistências nos dados de entrada, garantindo a robustez da solução.
* **Customização:** O código é facilmente adaptável para diferentes modelos de linguagem da Google ou para cenários de classificação mais específicos.
* **Análise de Gastos:** Permite categorizar automaticamente as transações do extrato do cartão de crédito, facilitando a identificação de padrões de gastos e o planejamento financeiro.

### Melhorias Futuras

* **Categorização Personalizada:** Permitir que o usuário defina suas próprias categorias e regras de classificação.
* **Aprendizado Contínuo:** Implementar um mecanismo para que o modelo aprenda com as correções do usuário, melhorando sua precisão ao longo do tempo.
* **Integração com Banco de Dados:**
    * **Input de Dados:** Permitir que os nomes dos estabelecimentos sejam lidos diretamente de um banco de dados, facilitando o processamento em lote e a integração com outras fontes de dados.
    * **Armazenamento de Resultados:** Salvar as categorias e justificativas geradas pelo modelo Gemini em um banco de dados, possibilitando análises mais aprofundadas, geração de relatórios e acompanhamento do desempenho do modelo ao longo do tempo.

### Como Usar (Google Colab)

1. **Abra o notebook no Colab:**
   * Acesse o Google Colab: [https://colab.research.google.com/](https://colab.research.google.com/)
   * Clique em "Arquivo" > "Abrir notebook" e selecione o arquivo `categorizador_inteligente.ipynb` do seu Google Drive ou faça upload dele.

2. **Configure sua Chave de API:**
   * Crie um arquivo chamado `credentials.json` na mesma pasta do seu notebook no Google Drive.
   * Insira sua chave de API do Google Cloud Console dentro desse arquivo.
   * No seu notebook, carregue as credenciais usando o seguinte código:

   ```python
   import os
   os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = "credentials.json"
   ```

3. **Execute as células do notebook:**
   * Clique no botão "Executar" (ícone de "play") em cada célula do notebook para executar o código em sequência.
   * Ou pressione `Shift + Enter` para executar a célula atual e passar para a próxima.

### Exemplo

```
Digite os nomes dos estabelecimentos (separados por vírgula): Padaria do Zé, Clínica Saúde & Vida, Restaurante Sabor da Terra, Uber, Netflix
```

Saída:

```
input: Padaria do Zé
output: Alimentação
output_justificativa: Padaria

input: Clínica Saúde & Vida
output: Saúde
output_justificativa: Clínica

input: Restaurante Sabor da Terra
output: Alimentação
output_justificativa: Restaurante

input: Uber
output: Transporte
output_justificativa: Serviço de transporte

input: Netflix
output: Entretenimento
output_justificativa: Serviço de streaming
```

### Tecnologias Utilizadas

* Python
* Google Generative AI
* Google Gemini

### Contribuição

Sinta-se à vontade para contribuir com melhorias, correções ou novos recursos!


