# Sistema MEWS Inteligente com IA 🧠🏥

Um projeto simples e divertido em Python para calcular o Score MEWS, salvar tudo no Google Drive e usar a Inteligência Artificial do Gemini para dar uma ajuda especial na interpretação e nas observações! ✨

---

## O Que é MEWS na Saúde? 🤔

Imagine que os médicos e enfermeiros no hospital precisam saber rapidinho se um paciente pode estar piorando, mesmo que ainda não pareça muito sério. Para isso, existe o **MEWS (Modified Early Warning Score)**!

É como um "sistema de alarme precoce" 🚨. Ele usa dados simples e importantes do paciente, como:

* Ritmo da respiração (FR - Frequência Respiratória) 💨
* Temperatura (Temp) 🌡️
* Pressão Arterial (PA) ❤️‍🩹
* Batimentos do coração (FC - Frequência Cardíaca) pulsando rápido ou devagar 💓
* Como o paciente está se sentindo ou respondendo (Nível de Consciência - NC) 😊😴

Cada um desses sinais recebe uma nota 🔢. Juntando todas as notas, dá um Score MEWS final. Quanto maior esse score, maior o risco e mais rápido a equipe precisa avaliar o paciente para garantir que ele fique bem! 👍

---

## Sobre o Projeto 💡

Este projeto é um script em Python, feito para rodar no Google Colab, que demonstra como podemos usar a tecnologia, incluindo Inteligência Artificial, para dar um suporte visual e contextual em ferramentas de saúde como o MEWS.

Ele não é um sistema médico oficial de hospital! 🙏 É uma forma de aprender e mostrar como a IA pode ajudar a organizar informações e destacar pontos importantes para a equipe de saúde, tornando o Score MEWS ainda mais útil. 😎

---

## Funcionalidades Top! ⭐

* **Calcula o Score MEWS Automaticamente:** Você insere os sinais vitais e ele calcula o score na hora, usando a tabela de pontuação padrão. 🔢
* **Salva o Histórico no Google Drive:** Cada monitorização (com score, sinais vitais e observações) é salva em uma planilha Excel no seu Google Drive. Seus dados ficam guardados! 💾📂
* **Histórico por Paciente:** Mostra o histórico de Scores e observações apenas do paciente que você está monitorando no momento. Os dados de outros pacientes ficam salvos, mas aparecem filtrados na tela. 🧍‍♀️🧍‍♂️
* **Visualização de Evolução:** Apresenta o histórico do paciente atual em formato de **tabela** (com bordas de texto simples para organizar ✨) e **gráfico** (para ver a tendência do score ao longo do tempo 📈📅).
* **Interpretação Inteligente com Gemini:** Usa a IA do Google Gemini (com sua chave API) para:
    * Gerar uma descrição amigável do que o score significa. 🗣️
    * Indicar quais sinais vitais mais contribuíram para o score.
    * **Sugere a ação a ser tomada com base no protocolo que VOCÊ define!** 📄👍
* **Análise de Observações com Gemini:** A IA lê as observações que você digitou e tenta extrair os pontos mais importantes e relevantes, como sintomas ou mudanças no paciente. 📝✨

---

## Como Funciona? 🛠️

* **Linguagem:** Python 🐍
* **Ambiente:** Google Colab (roda no seu navegador e já vem com as bibliotecas essenciais!) 🌐
* **Bibliotecas Principais:**
    * `pandas`: Para organizar e salvar os dados na planilha Excel. 📊
    * `matplotlib`: Para gerar o gráfico da evolução do score. 📈
    * `google-generativeai`: Para acessar a Inteligência Artificial do Google Gemini. 🤖
    * `google.colab`: Para conectar com o Google Drive e Secrets. ☁️🔑
    * `openpyxl`: Engine para o pandas ler/escrever arquivos `.xlsx`.
    * `pytz`: Para lidar com fusos horários (Embora a versão final aqui use timestamp simples, a biblioteca foi explorada!).
* **Armazenamento:** Planilha Excel (`.xlsx`) salva diretamente no seu Google Drive. 💾📂
* **IA:** Google Gemini API para análise de texto e geração de interpretação (requer sua chave API).

---

## Primeiros Passos 👋

1.  **Acesse o Código:** Abra este notebook no Google Colab.
2.  **Obtenha sua Chave API do Gemini:** Vá para o [Google AI Studio](https://aistudio.google.com/Huyprt/a/apikey) e crie uma chave de API. É rápido e fácil! 🔑
3.  **Salve a Chave API no Colab Secrets:**
    * No menu lateral esquerdo do Colab, clique no ícone de uma chave (🔑).
    * Clique em "Manage Secrets".
    * Clique em "New Secret".
    * No campo "Name", digite `API_KEY` (exatamente assim!).
    * No campo "Value", cole a sua chave de API.
    * Marque a opção "Notebook access" para este notebook.
    * Clique em "Done". **Pronto, sua chave está segura e não aparece no código!** 🔒
4.  **Crie a Pasta no Google Drive:** No seu Google Drive, crie uma pasta para guardar a planilha (ex: `DadosMEWS`).
5.  **Atualize o Caminho no Código:** No código Python, encontre a linha `excel_path = '/content/drive/My Drive/DadosMEWS/mews_pacientes.xlsx'` e altere `DadosMEWS` se você usou outro nome para a pasta.
6.  **Execute as Células:** Rode as células de código uma por uma, seguindo as instruções que aparecem no console na parte inferior.
7.  **Interaja com o Sistema:** Digite os dados solicitados (sinais vitais, observações, ID do paciente) no console e veja os resultados! 🚀

---

## Prints do Projeto Rodando! 📸
![image](https://github.com/user-attachments/assets/28aec533-630d-404c-b9db-a77614263983)


**1. Coletando os Dados do Paciente:**

*(Substitua a linha abaixo pelo código Markdown para sua imagem. Ex: `![Coleta de Dados](caminho/para/sua/imagem1.png)`)*

![image](https://github.com/user-attachments/assets/ef384817-d494-4015-82a4-8493d330bf7f)

![image](https://github.com/user-attachments/assets/6e618d22-dfee-4c7a-84c6-cc995ff26f70)

![image](https://github.com/user-attachments/assets/adca08b3-7218-4b20-acb6-cd2c784adc75)

![image](https://github.com/user-attachments/assets/89fafa04-7b1c-4a92-b5c5-4c72a50b7c01)



```markdown
![Coleta de Dados e Input](https://raw.githubusercontent.com/SEU_USUARIO/SEU_REPOSITORIO/main/caminho/para/sua/imagem_input.png)
