# Agente de Corrida — Guia Completo

> Meu treinador autônomo de Hyrox, corrida e musculação.
> Ele aprende com cada treino que eu envio e fica mais preciso com o tempo.

---

## O que este sistema faz

Você faz o Hyrox no seu espaço. Depois, manda o treino aqui. O agente lê, analisa o que foi cansado, olha seu histórico e gera o treino do dia seguinte — musculação e corrida — com tudo explicado.

**Entrada:** treino de Hyrox do dia
**Saída:** treino de academia + corrida para o dia seguinte, com razão e instrução técnica

---

## Como usar na prática

### PASSO 1 — Abrir esta pasta no Claude

Você precisa estar com a pasta **AGENTE DE CORRIDA** aberta como projeto no Claude Code.
Assim o Claude lê todos os arquivos automaticamente antes de responder.

> Se estiver usando o Claude no desktop app: a pasta já aparece no painel lateral quando configurada como projeto.

---

### PASSO 2 — Mandar o treino de Hyrox

Depois de fazer o Hyrox, mande uma mensagem para o Claude com o treino. Pode ser do jeito que preferir:

**Exemplo simples:**
> "Fiz Hyrox hoje. Estações: SkiErg 1000m, Sled Push, Lunges, Wall Balls. Cansaço 7."

**Exemplo completo (melhor para o agente):**
> "Fiz Hyrox hoje 24/11. Estações: SkiErg 1000m, Sled Push 50m, Remo 1000m, Farmers Carry, Wall Balls 100 reps. Cansaço geral 6, pernas pesadas, costas ok. Dormiu 6h."

**Pode mandar também:**
- Foto do quadro do treino
- Áudio (transcrito)
- Print do app do espaço Hyrox
- Texto simples — o agente interpreta

**Se o cansaço não for informado, o agente vai perguntar.**

---

### PASSO 3 — Receber o treino do dia seguinte

O agente vai gerar um treino completo com:

1. **Por que este treino** — o raciocínio baseado no seu Hyrox
2. **Musculação** — exercícios com séries, reps, carga sugerida, descanso e instrução técnica
3. **Corrida** — tipo do treino, aquecimento, parte principal com pace no Garmin, desaquecimento
4. **Dica do dia** — algo específico para você

---

### PASSO 4 — Dar feedback (opcional, mas poderoso)

Depois de fazer o treino gerado, mande como foi:

> "Fiz o treino. Musculação ok, supino consegui 42,5 kg. Corrida pesada, segurei o Z1 com dificuldade. Perna ainda doía do Hyrox. Cansaço 5."

O agente registra esse aprendizado e o próximo treino já vem mais calibrado.

---

## Mapa das pastas

| Pasta | O que guarda |
|---|---|
| `01-ATLETA` | Quem você é: perfil, metas, marcas pessoais, zonas |
| `02-AGENTES` | Os treinadores — instruções de como o Claude deve agir |
| `03-CONHECIMENTO` | A ciência por trás dos treinos: Hyrox, corrida, musculação |
| `04-TEMPLATES` | Modelos prontos para treinos e feedbacks |
| `05-TREINOS` | Diário completo — cada Hyrox e cada treino gerado |
| `06-PLANEJAMENTO` | Fase atual e calendário de provas |
| `07-EVOLUCAO` | Resumos semanais e aprendizados sobre o atleta |

---

## Arquivos mais importantes

| Arquivo | Por que ler |
|---|---|
| [[treinador-principal]] | Como o agente funciona por dentro |
| [[regras-de-combinacao]] | A lógica: Hyrox X → treino Y |
| [[perfil]] | Seus dados — atualizar se mudar algo |
| [[zonas-e-ritmos]] | Referência de pace para o Garmin |
| [[divisoes]] | Os dois treinos de academia disponíveis |

---

## Perguntas frequentes

**Posso mandar o Hyrox de qualquer jeito?**
Sim. Quanto mais detalhe, melhor o treino. Mas texto simples já funciona.

**E se não fizer Hyrox? Posso pedir treino assim mesmo?**
Sim. Manda uma mensagem tipo: "Não fiz Hyrox hoje. Pernas frescas. Qual treino faço amanhã?"

**E se quiser mudar algo no treino gerado?**
Fala direto: "Troca o agachamento por outro exercício" ou "Encurta a corrida, tenho 30 min".

**E se quiser priorizar corrida ou academia num dia específico?**
Avisa: "Amanhã quero focar só na corrida" ou "Quero um treino mais pesado de academia hoje".

**Quando o sistema fica mais inteligente?**
A cada feedback que você dá. O agente vai aprendendo o que funciona para você especificamente — cargas reais, ritmos reais, como você recupera.

---

## O que NÃO fazer

- Não pedir treino de Hyrox aqui — isso já está no seu espaço com o coach
- Não ignorar dor — se relatou dor, o agente vai reduzir carga. Não forçar.
- Não pular o feedback por semanas — o sistema fica cego sem ele

---

## Contato com o treinador

Basta abrir o Claude com esta pasta ativa e mandar uma mensagem. O agente responde em português, com linguagem profissional e clara. Pode perguntar qualquer coisa sobre os treinos, pedir ajustes ou tirar dúvidas técnicas.
