# 🎮 Criando um Dashboard de Vendas do Xbox com Excel

Este guia explica como estruturar uma planilha de controle e indicadores (Dashboard) do zero, utilizando as melhores práticas de organização de dados.

---

## 📂 Estrutura em Abas (O Segredo da Organização)

Para uma planilha profissional, não misture tudo. Organize seu arquivo utilizando o método ABCDE desenvolvido por Felipe Silva Aguiar da DIO, conforme detalhado a seguir: 

### 1. 🎨 Identidade Visual (`Assets`)
Para um visual profissional, separe os recursos: imagens, vídeos, gifs, paletas de cores, ícones e logos.
* **💡 Dica:** Mantenha um padrão de cores, use cores que remetam ao Xbox (Verde e Tons de Cinza/Preto) para que seu dashboard tenha uma identidade visual forte.

![Microsoft Excel - Dashboard Xbox](https://github.com/user-attachments/assets/b9b90c9a-3a32-4633-8c85-ec75c1407bdd)

### 2. 📊 Base de Dados (`Bases`)
É onde as informações "nascem". Aqui ficam os dados para gerar a dashboard principal e/ou outras medidas.
* **O que fazer:** Insira os dados em colunas (ex: ID, Data, Nome do Jogo, Categoria, Valor, Status).
* **💡 Dica:** Sempre formate o intervalo como **Tabela**, isso garante que, ao adicionar novos registros, os gráficos se atualizem sozinhos.

![Microsoft Excel - Dashboard Xbox_2](https://github.com/user-attachments/assets/1b3baa77-516d-4cc5-87a8-5715b33e898c)

### 3. 🧮 Inteligência e Fórmulas (`Cálculos`)
Aqui é o "motor" da planilha, onde os dados são processados para gerar informações.
* **O que fazer:** Para não poluir o visual, faça as contas aqui, crie Tabelas Dinâmicas para somar valores por categoria ou plataforma:
    - Vá em Inserir > Tabela Dinâmica.
    - Escolha os dados da aba "Bases".
    - Arraste os campos (ex: Arraste "Categoria" para Linhas e "Valor" para Valores).
    - Isso criará o resumo que alimentará seus gráficos.
* **Fórmulas Comuns:** - `=SOMA()` para totais.
    - `=CONT.SE()` para contar quantos jogos existem em cada categoria.
* Esta aba fica "escondida" do usuário final.

![Microsoft Excel - Dashboard Xbox_3](https://github.com/user-attachments/assets/8667af76-e042-4d6e-898a-2225bcc611d6)

### 4. 🕹️ Painel de Controle (`Dashboard`)
A parte visual que o usuário final interage.
* **Gráficos:** Use Gráficos Dinâmicos conectados à aba de Cálculos:
    - Clique na sua Tabela Dinâmica e vá em Análise de Tabela Dinâmica > Gráfico Dinâmico. Escolha modelos de barras, pizza ou linhas.
* **Filtros:** Use a **Segmentação de Dados** para criar botões interativos:
    - Vá em Inserir > Segmentação de Dados. Selecione "Categoria" ou "Plataforma". Isso criará botões clicáveis para filtrar o dashboard.
* **Design:** Remova as "Linhas de Grade" (Exibir > Desmarcar Linhas de Grade) para parecer um software, não uma planilha comum.

![Microsoft Excel - Dashboard Xbox_4](https://github.com/user-attachments/assets/b078fc8f-94ce-4a49-b79a-218ec386ecf5)

### 5. 🎨 Outros (`Extras`)
Aqui são armazenados os materiais de apoio, PDFs, documentos, estudos, etc.. Nem sempre é utilizado.

![Microsoft Excel - Dashboard Xbox_5](https://github.com/user-attachments/assets/b0620bfa-d2b7-4494-9872-d0fabeac5184)

---

## 🛠️ Passo a Passo Resumido

| Etapa | Ferramenta Excel | Objetivo |
| :--- | :--- | :--- |
| **Organizar** | Inserir Tabela | Manter dados padronizados e facilitar a gestão |
| **Resumir** | Tabela Dinâmica | Criar os números do dashboard |
| **Visualizar** | Gráficos | Facilitar a leitura rápida e clara de KPIs |
| **Filtrar** | Segmentação de Dados | Tornar o painel interativo |

---

*Projeto desenvolvido para o bootcamp Santander - Excel com Inteligência Artificial - 2º Semestre da DIO.*
