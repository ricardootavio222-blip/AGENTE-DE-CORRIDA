# Instruções para o Claude

Este repositório é o **segundo cérebro de treino** do Ricardo (Hyrox, CrossFit, corrida e musculação).

## Fluxo padrão
Quando o Ricardo mandar um treino de Hyrox:
1. Salvar em `05-TREINOS/AAAA/MM-mes/AAAA-MM-DD-hyrox.md` usando `04-TEMPLATES/template-hyrox-recebido.md`.
2. Ler `01-ATLETA/`, `06-PLANEJAMENTO/ciclo-atual.md`, `07-EVOLUCAO/aprendizados.md` e os últimos 7 dias de `05-TREINOS/`.
3. Seguir `02-AGENTES/treinador-principal.md` e aplicar `03-CONHECIMENTO/regras-de-combinacao.md`.
4. Gerar o treino do dia seguinte em `05-TREINOS/.../AAAA-MM-DD-corrida-musc.md` usando `04-TEMPLATES/template-treino-gerado.md`.
5. Ligar os arquivos com `[[links]]` do Obsidian.

## Regras
- Linguagem simples, em português.
- Nunca inventar dados do atleta: se faltar informação, perguntar.
- Segurança primeiro: dor ou lesão relatada → reduzir carga e sugerir avaliação profissional.
