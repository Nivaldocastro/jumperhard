# Godot RL Agents

Documentação do ambiente utilizado para desenvolvimento e treinamento de um agente de **Aprendizado por Reforço (Reinforcement Learning)** utilizando Godot, Python e Stable-Baselines3.

## 1. Projeto e Ambiente

O projeto utiliza o **Godot RL Agents** como integração entre o ambiente desenvolvido na Godot e o treinamento do agente em Python.

### Configuração

| Componente | Versão / Informação |
|---|---|
| Ambiente | JumperHard |
| Repositório | Godot RL Agents |
| Engine | Godot 4.7.2 (Mono/.NET) |
| Linguagem do ambiente | GDScript |
| Python | 3.10.11 |
| Framework de RL | Stable-Baselines3 2.4.0 |
| Algoritmo | PPO |
| Interface de ambiente | Gymnasium 1.0.0 |
| Biblioteca de integração | Godot RL Agents 0.8.2 |

### Repositório

O projeto utiliza o repositório oficial do **Godot RL Agents**:

https://github.com/edbeeching/godot_rl_agents

---

## 2. Bibliotecas Diretamente Envolvidas

As principais bibliotecas utilizadas no funcionamento do projeto são:

| Pacote | Versão | Utilização |
|---|---:|---|
| `godot_rl` | 0.8.2 | Comunicação entre o jogo no Godot e o treinamento em Python |
| `stable_baselines3` | 2.4.0 | Implementação do algoritmo de aprendizado por reforço |
| `gymnasium` | 1.0.0 | Interface e estrutura do ambiente de aprendizado por reforço |
| `torch` | 2.13.0 | Backend de aprendizado de máquina utilizado pelo Stable-Baselines3 |
| `numpy` | 1.26.4 | Operações numéricas e manipulação de dados |
| `cloudpickle` | 3.1.2 | Serialização utilizada no ecossistema do ambiente |
| `tqdm` | 4.70.0 | Barras de progresso durante os processos de treinamento |
| `tensorboard` | 2.21.0 | Monitoramento e visualização das métricas do treinamento |

---

## 3. Algoritmo de Aprendizado por Reforço

O algoritmo utilizado no treinamento do agente é o **PPO (Proximal Policy Optimization)**, disponibilizado pelo framework **Stable-Baselines3**.

A comunicação entre o ambiente desenvolvido na Godot e o treinamento realizado em Python é feita através da biblioteca **Godot RL Agents**.

### Tecnologias principais

- **Godot 4.7.2**
- **GDScript**
- **Python 3.10.11**
- **Godot RL Agents 0.8.2**
- **Stable-Baselines3 2.4.0**
- **Gymnasium 1.0.0**
- **PyTorch 2.13.0**
- **PPO**

---

## 4. Exportação e Execução do Modelo

Para a exportação e execução do modelo treinado, são utilizadas as seguintes bibliotecas:

| Pacote | Versão | Utilização |
|---|---:|---|
| `onnx` | 1.22.0 | Formato para exportação do modelo |
| `onnxruntime` | 1.23.2 | Execução de modelos no formato ONNX |
| `protobuf` | 7.36.0 | Serialização de dados utilizada por várias ferramentas do ecossistema |

O formato **ONNX (Open Neural Network Exchange)** é utilizado para permitir a exportação e execução do modelo treinado.

---

## 5. Bibliotecas Auxiliares

Além das bibliotecas diretamente relacionadas ao treinamento e à execução do modelo, o ambiente possui outras dependências auxiliares.

| Biblioteca | Versão |
|---|---:|
| `absl-py` | 2.5.0 |
| `certifi` | 2026.7.22 |
| `charset-normalizer` | 3.5.1 |
| `colorama` | 0.4.6 |
| `coloredlogs` | 15.0.1 |
| `contourpy` | 1.3.2 |
| `cycler` | 0.12.1 |
| `filelock` | 3.32.4 |
| `flatbuffers` | 25.12.19 |
| `fonttools` | 4.63.0 |
| `fsspec` | 2026.7.0 |
| `grpcio` | 1.83.0 |
| `huggingface_hub` | 0.36.2 |
| `huggingface-sb3` | 3.0 |
| `humanfriendly` | 10.0 |
| `idna` | 3.19 |
| `Jinja2` | 3.1.6 |
| `kiwisolver` | 1.5.0 |
| `Markdown` | 3.10.3 |
| `MarkupSafe` | 3.0.3 |
| `matplotlib` | 3.10.9 |
| `ml_dtypes` | 0.5.4 |
| `mpmath` | 1.3.0 |
| `networkx` | 3.4.2 |
| `packaging` | 26.3 |
| `pandas` | 2.3.3 |
| `pillow` | 12.3.0 |
| `pip` | 23.0.1 |
| `pyparsing` | 3.3.2 |
| `python-dateutil` | 2.9.0.post0 |
| `pytz` | 2026.3.post1 |
| `PyYAML` | 6.0.3 |
| `requests` | 2.34.2 |
| `setuptools` | 84.0.0 |
| `six` | 1.17.0 |
| `sympy` | 1.14.0 |
| `tensorboard-data-server` | 0.7.2 |
| `typing_extensions` | 4.16.0 |
| `tzdata` | 2026.3.post1 |
| `urllib3` | 2.7.0 |
| `wasabi` | 1.1.3 |
| `Werkzeug` | 3.1.8 |
| `wget` | 3.2 |

---

## 6. Estrutura Tecnológica

De forma geral, o projeto utiliza a seguinte estrutura:

```text
┌──────────────────────────────┐
│          Godot 4.7.2        │
│                              │
│       Ambiente JumperHard    │
│           GDScript           │
└──────────────┬───────────────┘
               │
               │ Godot RL Agents
               │
               ▼
┌──────────────────────────────┐
│          Python 3.10         │
│                              │
│       Gymnasium 1.0.0        │
│      Stable-Baselines3       │
│                              │
│             PPO              │
└──────────────┬───────────────┘
               │
               │ Treinamento
               ▼
┌──────────────────────────────┐
│       Modelo treinado        │
│                              │
│            ONNX              │
│        ONNX Runtime          │
└──────────────────────────────┘
