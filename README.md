<div align="center">

# 🧠 Cérebro Artificial Modular
## Emoções e Marcadores Somáticos

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**Uma simulação visualmente impressionante de um cérebro artificial modular baseado nas teorias de Paul Ekman e Antonio Damasio**

*"As emoções são estados corporais que guiam a tomada de decisão."* - Antonio Damasio

[🚀 Começar Agora](#-início-rápido) • [📖 Documentação](#-documentação-completa) • [🎨 Visualizações](#-galeria-de-visualizações) • [💡 Exemplos](#-exemplos-práticos)

---

</div>

## 📑 Índice de Navegação

<div align="center">

| [🎯 Sobre](#-sobre-o-projeto) | [🏗️ Arquitetura](#️-arquitetura-do-cérebro) | [🚀 Instalação](#-instalação) | [💻 Uso](#-como-usar) |
|:---:|:---:|:---:|:---:|
| [🎨 Visualizações](#-galeria-de-visualizações) | [📊 Recursos](#-recursos-e-funcionalidades) | [🔬 Teoria](#-fundamentação-teórica) | [🤝 Contribuir](#-contribuindo) |

</div>

---

## 🎯 Sobre o Projeto

### 🌟 O Que É?

Este projeto implementa um **cérebro artificial modular** que simula processos emocionais baseados em duas teorias fundamentais da neurociência:

<div align="center">

| **Paul Ekman** | **Antonio Damasio** |
|:---:|:---:|
| 😊 Emoções Básicas Universais | 🧬 Marcadores Somáticos |
| 6 emoções reconhecidas globalmente | Estados corporais que guiam decisões |
| Felicidade, Tristeza, Raiva, Medo, Surpresa, Neutro | Dopamina, Cortisol, Serotonina |

</div>

### ✨ Por Que Este Projeto?

- 🎨 **Visualizações 3D Impressionantes**: Veja o cérebro evoluindo em tempo real
- 🧠 **Baseado em Ciência Real**: Implementa teorias comprovadas da neurociência
- 📊 **Análise Multidimensional**: Dashboard completo com múltiplas métricas
- 🎬 **Animações Interativas**: Simulações em tempo real com gráficos dinâmicos
- 🔬 **Educacional**: Perfeito para aprender sobre neurociência computacional

---

## 🏗️ Arquitetura do Cérebro

### 🧩 Estrutura Modular

```
┌─────────────┐
│   ENTRADA   │  Eventos do ambiente
└──────┬──────┘
       │
       ├──────────────┬──────────────┐
       │              │              │
   ┌───▼───┐      ┌───▼───┐      ┌───▼───┐
   │Amígdala│      │Recomp.│      │Social │
   │Cortisol│      │Dopam. │      │Serot. │
   └───┬───┘      └───┬───┘      └───┬───┘
       │              │              │
       └──────────────┴──────────────┘
                      │
              ┌───────▼───────┐
              │  Marcadores   │
              │   Somáticos   │
              └───────┬───────┘
                      │
              ┌───────▼───────┐
              │  Memória LSTM │
              │   (Hipocampo) │
              └───────┬───────┘
                      │
              ┌───────▼───────┐
              │ Córtex Pré-   │
              │   Frontal     │
              └───────┬───────┘
                      │
              ┌───────▼───────┐
              │   EMOÇÃO      │
              │   FINAL       │
              └───────────────┘
```

### 🔴 Módulo 1: Amígdala (Sistema de Ameaça)

```python
🔴 Detecta: Perigo e estresse
📊 Atualiza: Cortisol (0-10)
⚡ Função: Resposta de luta ou fuga
```

### 🟢 Módulo 2: Sistema de Recompensa

```python
🟢 Detecta: Recompensas e prazer
📊 Atualiza: Dopamina (0-10)
⚡ Função: Motivação e aprendizado
```

### 🟡 Módulo 3: Marcadores Somáticos

```python
🟡 Estados: Dopamina, Cortisol, Serotonina
📊 Processa: Estados corporais internos
⚡ Função: Guiar tomada de decisão
```

### 🔵 Módulo 4: Memória Emocional (LSTM)

```python
🔵 Tipo: Long Short-Term Memory
📊 Tamanho: 8 neurônios ocultos
⚡ Função: Processar sequências temporais
```

---

## 🚀 Instalação

### 📋 Pré-requisitos

Certifique-se de ter instalado:

- **Python 3.8+** 
- **Jupyter Notebook** ou **JupyterLab**
- **Git** (opcional)

### 🔧 Passo a Passo

#### 1️⃣ Clone o Repositório

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/cerebro-emocional.git
cd cerebro-emocional
```

#### 2️⃣ Instale as Dependências

```bash
pip install torch matplotlib numpy seaborn scipy
```

Ou usando `requirements.txt`:

```bash
pip install -r requirements.txt
```

#### 3️⃣ Abra o Jupyter Notebook

```bash
jupyter notebook cerebro_emocional.ipynb
```

### ✅ Verificação

Execute a primeira célula para verificar se tudo está funcionando:

```python
import torch
import numpy as np
import matplotlib.pyplot as plt

print("✅ Tudo pronto!")
print(f"PyTorch: {torch.__version__}")
print(f"NumPy: {np.__version__}")
```

---

## 💻 Como Usar

### 🎯 Uso Básico

#### 1. Criar uma Instância do Cérebro

```python
from cerebro_emocional import CerebroEmocional

cerebro = CerebroEmocional()
```

#### 2. Simular um Evento

```python
# Evento: Recebeu um presente
cerebro.atualizar_estado(
    recompensa=2.0,  # Aumenta dopamina
    ameaca=0.0,       # Sem ameaça
    social=1.0        # Interação social positiva
)
```

#### 3. Prever a Emoção

```python
resultado = cerebro.prever_emocao()

print(f"Emoção: {resultado['emoji']} {resultado['emocao']}")
print(f"Confiança: {max(resultado['probabilidades'])*100:.1f}%")
```

### 📊 Exemplo Completo

```python
# Criar cérebro
cerebro = CerebroEmocional()

# Simular uma sequência de eventos
eventos = [
    {"nome": "Recebeu presente", "recompensa": 2.0, "ameaca": 0.0, "social": 1.0},
    {"nome": "Viu predador", "recompensa": 0.0, "ameaca": 3.0, "social": 0.0},
    {"nome": "Encontrou amigo", "recompensa": 1.0, "ameaca": 0.0, "social": 2.0},
]

# Processar eventos
for evento in eventos:
    cerebro.atualizar_estado(
        recompensa=evento["recompensa"],
        ameaca=evento["ameaca"],
        social=evento["social"]
    )
    
    resultado = cerebro.prever_emocao()
    print(f"{evento['nome']}: {resultado['emoji']} {resultado['emocao']}")
```

---

## 🎨 Galeria de Visualizações

### 📈 1. Gráficos Temporais

<div align="center">

**Evolução dos Marcadores Somáticos ao Longo do Tempo**

```
Dopamina  ████████████████████░░░░░░░░░░  8.5
Cortisol  ████████░░░░░░░░░░░░░░░░░░░░░░  3.2
Serotonina ████████████░░░░░░░░░░░░░░░░░  5.8
```

</div>

### 🌐 2. Visualização 3D

**Espaço Tridimensional dos Estados Emocionais**

- 🟢 Eixo X: Dopamina
- 🔴 Eixo Y: Cortisol  
- 🟡 Eixo Z: Serotonina

### 🧠 3. Cérebro 3D com Mapa de Calor

**Representação Visual do Cérebro com Emoções**

- Cada região colorida pela emoção ativa
- Intensidade representada pelo brilho
- Padrões de ondas simulando atividade neural

### 📊 4. Dashboard Completo

**Análise Multidimensional com 10+ Gráficos**

- 📈 Evolução temporal
- 🔥 Matriz de correlação
- 📦 Box plots comparativos
- 🎻 Gráficos de violino
- 🎯 Gráficos de radar

### 🎬 5. Animações em Tempo Real

**Simulação Completa com 6 Painéis Simultâneos**

- Gráfico temporal animado
- Visualização 3D dinâmica
- Barras de estados atualizadas
- Probabilidades emocionais
- Informações detalhadas
- Gráfico radar interativo

---

## 📊 Recursos e Funcionalidades

### 🎯 Funcionalidades Principais

<div align="center">

| Funcionalidade | Descrição | Status |
|:---:|:---|:---:|
| 🧠 **Modelo Neural** | LSTM para memória emocional | ✅ |
| 📊 **Visualizações 3D** | Cérebro com mapas de calor | ✅ |
| 🎬 **Animações** | Simulações em tempo real | ✅ |
| 📈 **Dashboards** | Análise multidimensional | ✅ |
| 🎨 **Gráficos** | 15+ tipos diferentes | ✅ |
| 🔬 **Análise** | Estatísticas completas | ✅ |

</div>

### 🎨 Tipos de Visualizações

#### 📊 Gráficos Estáticos

- ✅ Gráficos de linha (evolução temporal)
- ✅ Gráficos de barras (estados atuais)
- ✅ Gráficos de área empilhada
- ✅ Heatmaps de correlação
- ✅ Box plots comparativos
- ✅ Gráficos de violino
- ✅ Histogramas de distribuição
- ✅ Gráficos de radar (spider charts)

#### 🌐 Visualizações 3D

- ✅ Espaço 3D dos estados
- ✅ Cérebro com mapa de calor uniforme
- ✅ Cérebro com ativação regional
- ✅ Cérebro com todas as emoções
- ✅ Cérebro com gradiente radial
- ✅ Cérebro com padrão de ondas
- ✅ Múltiplas vistas (frontal, lateral, superior)

#### 🎬 Animações

- ✅ Animação temporal dos estados
- ✅ Animação 3D do espaço emocional
- ✅ Animação do cérebro evoluindo
- ✅ Dashboard animado completo

---

## 🔬 Fundamentação Teórica

### 📚 Paul Ekman - Emoções Básicas

**Teoria**: Existem 6 emoções universais reconhecidas em todas as culturas.

<div align="center">

| Emoção | Emoji | Cor | Função |
|:---:|:---:|:---:|:---|
| **Felicidade** | 😊 | 🟡 Amarelo | Prazer e satisfação |
| **Tristeza** | 😢 | 🔵 Azul | Perda e desapontamento |
| **Raiva** | 😠 | 🔴 Vermelho | Frustração e agressão |
| **Medo** | 😨 | 🟣 Roxo | Ansiedade e alerta |
| **Surpresa** | 😲 | 🟠 Laranja | Inesperado e choque |
| **Neutro** | 😐 | ⚪ Cinza | Estado base |

</div>

### 🧬 Antonio Damasio - Marcadores Somáticos

**Hipótese**: As emoções são estados corporais que guiam a tomada de decisão racional.

#### 🟢 Dopamina

```
Função: Sistema de recompensa
Efeito: Prazer, motivação, aprendizado
Ativação: Recompensas positivas
```

#### 🔴 Cortisol

```
Função: Sistema de estresse
Efeito: Alerta, ansiedade, resposta de luta/fuga
Ativação: Ameaças e perigos
```

#### 🟡 Serotonina

```
Função: Bem-estar social
Efeito: Humor, interação social, estabilidade
Ativação: Conexões sociais positivas
```

### 🧮 Modelo Matemático

#### Equações de Atualização

```
dopamina(t+1) = dopamina(t) + recompensa - 0.1 × dopamina(t)
cortisol(t+1) = cortisol(t) + ameaça - 0.1 × cortisol(t)
serotonina(t+1) = serotonina(t) + social - 0.05 × serotonina(t)
```

#### Processamento Neural

```
estado = [dopamina, cortisol, serotonina]
memoria = LSTM(estado)
emocao = Softmax(Linear(memoria))
```

---

## 🎓 Exemplos Práticos

### 📖 Exemplo 1: Um Dia na Vida

```python
historia = [
    {"evento": "Acordou descansado", "recompensa": 0.5, "ameaca": 0.0, "social": 0.0},
    {"evento": "Tomou café da manhã", "recompensa": 1.0, "ameaca": 0.0, "social": 0.0},
    {"evento": "Chegou atrasado", "recompensa": 0.0, "ameaca": 1.5, "social": -0.5},
    {"evento": "Recebeu elogio", "recompensa": 2.0, "ameaca": 0.0, "social": 1.0},
]

for momento in historia:
    cerebro.atualizar_estado(
        recompensa=momento["recompensa"],
        ameaca=momento["ameaca"],
        social=momento["social"]
    )
    resultado = cerebro.prever_emocao()
    print(f"{momento['evento']}: {resultado['emoji']} {resultado['emocao']}")
```

**Saída Esperada:**

```
Acordou descansado: 😐 neutro
Tomou café da manhã: 😊 feliz
Chegou atrasado: 😨 medo
Recebeu elogio: 😊 feliz
```

### 🎮 Exemplo 2: Simulação de Cenários

```python
# Cenário: Vitória em competição
cerebro.atualizar_estado(recompensa=3.0, ameaca=0.0, social=1.5)
# Resultado: 😊 Feliz (alta confiança)

# Cenário: Conflito social
cerebro.atualizar_estado(recompensa=0.0, ameaca=2.0, social=-1.0)
# Resultado: 😠 Raiva ou 😨 Medo

# Cenário: Reencontro com amigo
cerebro.atualizar_estado(recompensa=1.0, ameaca=0.0, social=2.5)
# Resultado: 😊 Feliz (alta serotonina)
```

---

## 🎨 Interface e Experiência do Usuário

### 🌙 Design Dark Mode

Todas as visualizações usam um **tema escuro moderno** para:

- ✅ Reduzir fadiga visual
- ✅ Melhorar contraste
- ✅ Experiência profissional
- ✅ Compatibilidade com ambientes de baixa luz

### 📱 Layout Responsivo

Os gráficos são otimizados para:

- 💻 **Desktop**: Visualizações completas em alta resolução
- 📊 **Jupyter**: Integração perfeita com notebooks
- 🖼️ **Exportação**: Qualidade para apresentações

### 🎯 Interatividade

- 🖱️ **Zoom**: Amplie áreas de interesse
- 🔄 **Rotação 3D**: Explore diferentes ângulos
- ⏯️ **Animações**: Controle de velocidade e pausa
- 📊 **Tooltips**: Informações detalhadas ao passar o mouse

---

## 📈 Métricas e Análises

### 📊 Estatísticas Disponíveis

<div align="center">

| Métrica | Descrição | Exemplo |
|:---:|:---|:---:|
| **Média** | Valor médio dos estados | Dopamina: 4.2 |
| **Máximo** | Pico de ativação | Cortisol: 8.5 |
| **Mínimo** | Estado mais baixo | Serotonina: 1.2 |
| **Correlação** | Relação entre estados | Dop×Cort: -0.3 |
| **Confiança** | Certeza da previsão | 87.5% |

</div>

### 🔍 Análises Avançadas

- 📊 **Matriz de Correlação**: Relações entre marcadores
- 📈 **Distribuições**: Histogramas e densidades
- 🎯 **Tendências**: Padrões temporais
- 📉 **Variabilidade**: Mudanças emocionais

---

## 🛠️ Tecnologias Utilizadas

<div align="center">

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white)

</div>

### 📦 Dependências Principais

| Biblioteca | Versão | Uso |
|:---:|:---:|:---|
| **PyTorch** | 2.0+ | Redes neurais (LSTM) |
| **NumPy** | 1.20+ | Computação numérica |
| **Matplotlib** | 3.5+ | Visualizações 2D/3D |
| **SciPy** | 1.7+ | Interpolação e análise |
| **Seaborn** | 0.11+ | Estatísticas visuais |

---

## 🚀 Performance

### ⚡ Otimizações

- 🎯 **Processamento Eficiente**: Cálculos vetorizados com NumPy
- 🧠 **GPU Ready**: Suporte para CUDA (PyTorch)
- 📊 **Renderização Rápida**: Gráficos otimizados
- 💾 **Memória Eficiente**: Gerenciamento inteligente de dados

### 📊 Benchmarks

```
Simulação de 100 eventos: ~0.5 segundos
Geração de dashboard: ~2 segundos
Animação completa (8 frames): ~8 segundos
```

---

## 🎓 Casos de Uso

### 🎓 Educacional

- **Neurociência Computacional**: Aprenda sobre modelos emocionais
- **Machine Learning**: Entenda LSTM e classificação
- **Visualização de Dados**: Explore técnicas avançadas

### 🔬 Pesquisa

- **Modelagem Emocional**: Base para pesquisas em IA emocional
- **Análise Comportamental**: Simulação de respostas emocionais
- **Interface Humano-Computador**: Sistemas mais empáticos

### 💼 Aplicações Práticas

- **Gamificação**: Sistemas de recompensa em jogos
- **Assistentes Virtuais**: Respostas mais naturais
- **Análise de Sentimentos**: Compreensão emocional avançada

---

## 🤝 Contribuindo

### 🌟 Como Contribuir

1. **Fork** o projeto
2. **Crie** uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. **Commit** suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. **Push** para a branch (`git push origin feature/AmazingFeature`)
5. **Abra** um Pull Request

### 📝 Sugestões de Melhorias

- ✨ Adicionar mais marcadores somáticos (adrenalina, ocitocina)
- 🎯 Implementar aprendizado por reforço
- 🧠 Adicionar mecanismo de atenção
- 🌐 Criar interface web interativa
- 📱 Desenvolver app mobile

---

## 📚 Referências Científicas

### 📖 Artigos e Livros

1. **Ekman, P. (1992)**
   - "An argument for basic emotions"
   - *Cognition & Emotion*, 6(3-4), 169-200

2. **Damasio, A. (1994)**
   - "Descartes' Error: Emotion, Reason, and the Human Brain"
   - *Putnam Publishing*

3. **LeCun, Y., Bengio, Y., & Hinton, G. (2015)**
   - "Deep learning"
   - *Nature*, 521(7553), 436-444

---

## 📝 Licença

Este projeto está licenciado sob a **MIT License**.

```
MIT License

Copyright (c) 2026 [Seu Nome]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

## 👤 Autor

<div align="center">

### **Pedro Victor Rocha Gonçalves**

**Desenvolvedor | Pesquisador em Neurociência Computacional | Entusiasta de IA**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pedro-victor-rocha-gon%C3%A7alves-751b38294/)

*"Transformando conceitos complexos da neurociência em visualizações compreensíveis e interativas."*

</div>

---

## 🌟 Agradecimentos

- 🧠 **Paul Ekman** - Por suas pesquisas sobre emoções universais
- 🧬 **Antonio Damasio** - Por sua teoria dos marcadores somáticos
- 🐍 **Comunidade Python** - Pelas ferramentas incríveis
- 📚 **Neurocientistas** - Por inspirar este projeto

---

<div align="center">

### ⭐ Se este projeto foi útil, considere dar uma estrela!

[⬆ Voltar ao topo](#-cérebro-artificial-modular)

**Feito com ❤️ e 🧠 usando Python, PyTorch e muito café ☕**

---

!
</div>

