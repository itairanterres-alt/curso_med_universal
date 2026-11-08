# Santa Casa/UFCSPA 2027 — Auditoria: resolução própria (Claude) × gabarito × V2 do ChatGPT

Data: 08/11/2026. Material em rascunho, oculto ao estudante (`student_visible = false`).

## 1. Método e limites

1. **Resolução própria das 100 questões** diretamente do PDF da prova (`UFCSPA-Medica-ACESSO-DIRETO.pdf`), com leitura das figuras originais (ECG da Q30 e forest plot da Q58). Cada item tem resposta, nível de confiança, justificativa, comentário das quatro alternativas, flashcard (ou decisão justificada de não criar) e ressalva. O texto é original; não reaproveita a redação da V1 nem da V2.
2. **A resolução não foi cega.** Antes de redigir, eu já tinha visto as letras do gabarito preliminar e os comentários da V1 sobre as 11 questões que ela bloqueou. Por isso, a concordância com o gabarito não é medida independente de acurácia. O que pode ser verificado é a fundamentação escrita de cada item.
3. **Confronto com o gabarito preliminar** (Edital nº 06, 04/11/2026). A cópia do Drive e a publicação da FUNDMED são idênticas. O gabarito definitivo ainda não foi publicado.
4. **Auditoria cruzada com a V2 do ChatGPT** (`Santa_Casa_2027_Medunidavi_V2_RASCUNHO.zip`, no Drive), feita **depois** de redigir os 100 itens: respostas, decisões editoriais, ressalvas e pendências documentais.
5. **Limitação de fontes.** Nesta sessão, as referências foram citadas a partir do conhecimento das diretrizes e tratados, sem abrir cada documento. Os itens marcados com confiança "moderada" ou com "conferir" na ressalva precisam de verificação documental antes da publicação. Nesse quesito, a V2 é superior: ela registra a fonte efetivamente lida para cada campo.

## 2. Resultado

| Indicador | Resolução Claude | V2 ChatGPT |
|---|---|---|
| Itens com justificativa e comentário A–D | 100 | 100 |
| Concordância da resposta com o gabarito preliminar | 95/100 | 91/100 (AMBIGUOUS ou divergente em 9) |
| Flashcards | 95 (5 itens sem cartão, todos de competência atitudinal ou memorização pura) | 85 |
| Itens bloqueados | 5 (28, 38, 52, 88, 90) | 10 (28, 33, 35, 38, 52, 58, 86, 88, 90, 100) |
| Itens liberáveis com nota | 34 | 23 com *caveat* |
| Fonte lida registrada por campo | Não | Sim (`fontes_e_cobertura.csv`) |

### Divergências entre a minha resolução e o gabarito preliminar
| Q | Gabarito | Claude | Motivo |
|---|:-:|:-:|---|
| 28 | B | nenhuma | CURB-65 = 3, não 4. B acerta a conduta e erra o escore; 22% é a mortalidade do grupo 3–5. |
| 38 | D | C | No fluxograma do Ministério da Saúde, TR-HBsAg reagente é complementado com HBV-DNA. |
| 52 | A | nenhuma | Só a afirmativa I é correta; não há alternativa "apenas I". |
| 88 | C | A ou C | A vinheta não discrimina invaginação de Meckel com segurança. |
| 90 | B | nenhuma | Com SpO₂ de 94–95%, as diretrizes não indicam O₂; B não tem sustentação. |

A V2 chega às mesmas conclusões nesses cinco itens (Q38 = C; os demais retidos como AMBIGUOUS). São as **candidatas a anulação ou alteração** quando sair o gabarito definitivo.

## 3. Onde eu e a V2 divergimos (5 itens)

| Q | V2 | Claude | Avaliação |
|---|---|---|---|
| **33** (gota) | Retida: C impõe colchicina como preferencial, contra o ACR 2020 | C, liberável com nota | A objeção da V2 é correta como regra geral. Mas o paciente é diabético e hipertenso, em uso de IECA e tiazídico, o que torna o AINE relativamente contraindicado e a colchicina a escolha contextual. Proponho liberar com nota sobre os três agentes de primeira linha. **Decisão do curador.** |
| **35** (SDRA) | Fonte central pendente: a afirmação de A não estava no resumo do LUNG SAFE | A, confiança moderada | A frase de A ("mortalidade quase duas vezes maior por causa direta") vem da seção de prognóstico da SDRA no **Harrison**, que também sustenta a falsidade de B, C e D (≈ 9–16% das mortes por insuficiência respiratória; idade como fator de risco; PEEP e complacência descartadas em Berlim). A menção a "LUNG SAFE" no enunciado é imprecisa. **Ação: conferir a página do Harrison e, se confirmada, liberar com nota.** |
| **58** (forest plot) | Retida: figura de doença cardiovascular, pergunta sobre HAS | B, liberável com nota | Concordo com o defeito de desfecho. Como treino de leitura de forest plot, B é a única leitura estatística correta. Detalhe que a V2 não registrou: a premissa de C é verdadeira (só Ciruzzi 1998 e McElduff 1998, sexo feminino, não cruzam 1); a conclusão é que é falsa. **Decisão do curador.** |
| **86** (mecônio) | Retida: C recomenda aspiração sem condicionar à obstrução | D, liberável com nota | A alternativa C reproduz a diretriz da **SBP** para RN ≥ 34 semanas, referência natural de uma banca brasileira. D é inequivocamente a incorreta. A divergência SBP × ILCOR/AHA vai para a nota, sem bloquear. |
| **100** (DM1) | Fonte central pendente | C, confiança moderada | Concordo que é preciso conferência documental. O raciocínio que sustenta C: a perda de peso precede o diagnóstico clínico por insulinopenia, enquanto crescimento linear e ganho ponderal acelerados aparecem anos antes, na fase pré-clínica (DAISY, TEDDY). **Ação: conferir antes de publicar.** |

## 4. O que a V2 apontou e eu incorporei

- **Q53:** encontrar indivíduos integrados entre os suicidas não invalida, por si só, a associação coletiva. Ressalva adicionada.
- **Q55** (e Q54): o desaparecimento da associação após estratificação é dado didático do enunciado, não resultado conferido de MacMahon (1981). Ressalva adicionada.
- **Q19:** a V2 registra que o percentual "¾" da alternativa C não tem fonte. Minha redação já trata C como "proporção sem sustentação".

## 5. O que eu encontrei e a V2 não registra

- **Q35:** identificação da provável fonte textual (Harrison) que sustenta a alternativa A e refuta as demais.
- **Q58:** a premissa da alternativa C é factualmente verdadeira (exatamente dois estudos significativos); o erro está na inferência.
- **Q25:** o déficit corporal de K⁺ com K⁺ de 2 mEq/L é de 300–600 mEq, o que torna B falsa pela ordem de grandeza.
- **Q42:** a alternativa D é cópia literal da D da Q41 (erro de diagramação da banca).
- **Q62:** a alternativa D também é factualmente errada ao classificar o clonazepam como de "meia-vida mais curta".
- **Q71:** o teste de aminas (*whiff*) é feito com KOH, não "no microscópio".

## 6. Autocrítica da minha versão

- **Itens com confiança moderada ou baixa**, que pedem conferência documental: 13, 20, 33, 35, 62, 88, 100. Itens com dependência de diretriz recente: 22 (SBC 2025), 89 (GINA 2026) e 97 (nota técnica do MS de 2026).
- **Sem rastreabilidade por campo.** Para publicação, cada justificativa deve ser cruzada com o `fontes_e_cobertura.csv` da V2 ou receber fonte própria conferida.
- **Flashcards:** criei 95, contra 85 na V2, que removeu 15 cartões por redundância ou ambiguidade. Na curadoria, convém comparar os cartões dos itens em que a V2 removeu o seu.

## 7. Recomendação para a curadoria

1. Usar como base a minha versão ou a V2, conforme a preferência editorial. Elas concordam em 95 dos 100 itens quanto à resposta.
2. Decidir os 5 itens de divergência (seção 3).
3. Manter bloqueados 28, 38, 52, 88 e 90 até o gabarito definitivo.
4. Conferir as fontes dos itens listados na seção 6 antes de liberar ao estudante.
