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
```
# JumperHard — Documentação Técnica do Treinamento

## 1. Visão geral

O **JumperHard** é um ambiente tridimensional desenvolvido no Godot para treinar um agente por meio de Aprendizado por Reforço (*Reinforcement Learning*). O objetivo do agente é movimentar o personagem e realizar saltos para alcançar plataformas distribuídas pelo cenário.

O treinamento utiliza o algoritmo **PPO (Proximal Policy Optimization)**, integrado ao ambiente por meio do Godot RL Agents e do Stable-Baselines3.

O projeto também registra métricas por episódio para permitir a comparação entre treinamentos e a construção de um dataset com os resultados obtidos.

## 2. Algoritmo e configuração

| Item | Descrição |
|---|---|
| Projeto | JumperHard |
| Abordagem | Aprendizado por Reforço |
| Algoritmo | PPO (*Proximal Policy Optimization*) |
| Ambiente | Godot 3D |
| Integração | Godot RL Agents |
| Biblioteca de treinamento | Stable-Baselines3 |
| Ambientes previstos | 16 |
| Meta de episódios | 100 por ambiente |

Os hiperparâmetros específicos, como `total_timesteps`, `n_steps` e `ent_coef`, devem ser registrados individualmente para cada experimento, conforme a configuração realmente utilizada.

## 3. Parâmetros físicos do jogador

Os seguintes parâmetros estão definidos no script `Player.gd`:

| Parâmetro | Valor | Descrição |
|---|---:|---|
| `MOVE_SPEED` | 12 | Velocidade de movimento |
| `JUMP_FORCE` | 30 | Força inicial do salto |
| `GRAVITY` | 0.98 | Decremento aplicado à velocidade vertical por atualização física |
| `MAX_FALL_SPEED` | 30 | Limite da velocidade de queda |
| `TURN_SENS` | 4.0 | Sensibilidade da rotação |

No início de cada episódio, o jogador é posicionado em `(0, 5, 0)`, e sua rotação em torno do eixo Y é sorteada entre -180° e 180°.

A primeira plataforma é posicionada em `(0, 0, 0)`, enquanto a segunda começa em `(0, 0, -12)`.

Após o alcance de uma plataforma, a posição da próxima é calculada utilizando uma distância aleatória entre 12 e 16 unidades e um ângulo aleatório entre -180° e 180°.

## 4. Entradas do agente — Observações

O agente recebe informações do ambiente por meio da função `get_obs()`, implementada em `AIController3D.gd`.

### 4.1 Vetor de observações

| Entrada | Descrição | Normalização |
|---|---|---|
| Velocidade X | Componente horizontal da velocidade | Dividida por `MOVE_SPEED` |
| Velocidade Y | Componente vertical da velocidade | Dividida por `MAX_FALL_SPEED` |
| Velocidade Z | Componente longitudinal da velocidade | Dividida por `MOVE_SPEED` |
| Distância ao objetivo | Distância entre o jogador e a plataforma-alvo | Limitada a 20 unidades e dividida por 20 |
| Direção X | Componente X da direção relativa ao objetivo | Vetor normalizado |
| Direção Y | Componente Y da direção relativa ao objetivo | Vetor normalizado |
| Direção Z | Componente Z da direção relativa ao objetivo | Vetor normalizado |
| `grounded` | Indica se o jogador está no chão | Valor booleano |
| Sensor de raios | Informações retornadas por `RayCastSensor3D` | Conforme a configuração do sensor |

O vetor contém **8 componentes explícitos**, além dos valores fornecidos pelo sensor de raios.

A dimensão total das observações é:

`8 + N`

em que `N` representa a quantidade de valores retornados pelo `RayCastSensor3D`.

### 4.2 Posição do jogador e das plataformas

As posições globais do jogador e da plataforma-alvo são utilizadas internamente para calcular a distância e a direção relativa.

Entretanto, as coordenadas absolutas X, Y e Z dessas posições não são adicionadas diretamente ao vetor de observações apresentado no código.

A direção do objetivo é transformada para o referencial local do jogador e normalizada antes de ser fornecida ao agente.

## 5. Saídas do agente — Ações

O espaço de ações declarado no controlador contém três ações contínuas:

| Ação | Descrição |
|---|---|
| `move` | Controla o movimento longitudinal do jogador, com valor limitado entre -1 e 1 |
| `jump` | Controla o comando de salto; valores maiores que zero ativam a ação |
| `turn` | Está declarado no espaço de ações, mas a saída correspondente não é utilizada diretamente no `set_action()` fornecido |

**Observação:** no código atual, a rotação do jogador é calculada automaticamente com base na direção da plataforma-alvo. O controlador ajusta o giro conforme o ângulo relativo e interrompe a correção quando o personagem está alinhado a menos de 8° do objetivo.

Assim, a saída `turn` está declarada, mas o giro efetivamente executado é calculado por uma regra geométrica.

## 6. Função de recompensa

A função `update_reward()` é responsável por atualizar a recompensa do agente.

| Evento | Recompensa |
|---|---:|
| Penalidade por atualização física | -0.01 |
| Aproximação do objetivo | Diferença positiva entre a melhor distância anterior e a distância atual |
| Alcance de uma plataforma válida | +100.0 |
| Queda ou término do episódio | Encerramento do episódio, sem bônus específico de queda nos trechos documentados |

### 6.1 Recompensa por aproximação

O sistema compara a distância atual até a plataforma-alvo com a menor distância registrada anteriormente.

Quando o jogador alcança uma distância menor, a diferença é adicionada à recompensa e a melhor distância é atualizada.

Quando o objetivo muda, a referência de distância é reinicializada para acompanhar a nova plataforma-alvo.

### 6.2 Recompensa por alcançar plataformas

O sistema alterna entre duas plataformas:

1. A primeira plataforma é aceita quando `next == 0`.
2. Após alcançá-la, o contador de plataformas aumenta e o objetivo passa a ser a segunda plataforma.
3. A segunda plataforma é aceita quando `next == 1`.
4. Após alcançá-la, o objetivo volta a ser a primeira plataforma.

Cada alcance válido adiciona `+100.0` à recompensa.

### 6.3 Pontuação acumulada

A função `get_reward()` acumula as recompensas recebidas durante o episódio em `pontuacao_total_episodio`, zera a recompensa pendente e retorna o valor ao sistema de treinamento.

No encerramento do episódio, a pontuação final considera a soma acumulada e a recompensa que ainda estiver pendente.

Atualmente, essa pontuação é exibida no console, mas não está incluída no CSV de métricas.

## 7. Métricas por episódio

O projeto registra informações que permitem analisar o comportamento do agente durante o treinamento.

| Métrica | Descrição |
|---|---|
| `treinamento` | Identificador do treinamento |
| `ambiente` | Identificador do ambiente |
| `episodio` | Número do episódio |
| `plataformas_alcancadas` | Quantidade de plataformas alcançadas |
| `tempo_sobrevivido` | Tempo de sobrevivência em segundos |
| `pulos_realizados` | Quantidade de saltos iniciados |
| `motivo_termino` | Motivo informado para o encerramento |

O arquivo é criado em `user://metricas_treinamento.csv`.

O cabeçalho atual é:

```csv
treinamento,ambiente,episodio,plataformas_alcancadas,tempo_sobrevivido,pulos_realizados,motivo_termino
```

O identificador inicial definido no código para o treinamento é `100eps`.

A pontuação total é calculada e exibida no console, mas ainda não é salva nesse arquivo. Caso seja utilizada como variável do dataset, será necessário acrescentar a coluna correspondente à função de gravação.

## 8. Controle e encerramento dos episódios

O projeto estabelece uma meta de 100 episódios para cada um dos 16 ambientes.

A contagem dos episódios é mantida por ambiente, permitindo verificar o progresso individual de cada instância.

Quando um ambiente alcança a meta, ele é marcado como finalizado e deixa de iniciar novos episódios. O encerramento global ocorre quando todos os ambientes previstos estão registrados e atingem a quantidade mínima de episódios estabelecida.

O cumprimento dessa meta indica que o critério de execução foi alcançado, mas não garante, isoladamente, que a política aprendida seja ótima. A avaliação deve considerar as métricas e a comparação entre os experimentos.

## 9. Organização dos modelos e experimentos

Os modelos foram organizados de forma a pegar o último arquivo de checkpoint de cada treinamento  
```text
JumperHard/
├── logs/sb3/   
│         ├── checkpoint/
│         │   ├── checkpoint_escolhido1.zip
│         │   └── checkpoint_escolhido2.zip
│         │   └── checkpoint_escolhido3.zip
|         |   
│         ├── experiment_1/
│         │   ├── checkpoints_1000_steps.zip
│         │   └── checkpoints_2000_steps.zip
|         ├── experiment_2/
│         │   ├── checkpoints_4000_steps.zip
│         │   └── checkpoints_5000_steps.zip
│         └── ...
├── metricas_treinamento.csv
└── README.md
```

