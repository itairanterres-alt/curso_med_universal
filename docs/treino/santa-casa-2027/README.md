# Santa Casa/UFCSPA 2027 — Acesso Direto: material para o treino MEDUNIDAVI

**Situação:** RASCUNHO EDITORIAL, sem liberação ao estudante (`student_visible = false` em todos os registros).

| Item | Quantidade |
|---|---|
| Questões comentadas (justificativa + comentário por alternativa) | 100 |
| Flashcards | 94 |
| Questões com ressalva editorial | 51 |
| Questões bloqueadas | 11 (13, 20, 28, 35, 38, 52, 58, 86, 88, 90, 97) |
| Concordância da resolução cega com o gabarito | 93/100 |

## Fontes

- Prova: [UFCSPA-Medica-ACESSO-DIRETO.pdf](https://drive.google.com/file/d/184wAibaUuAJcpkbtZ278HfPk7dmhIqAf/view)
- Gabarito **preliminar** (Edital nº 06, 04/11/2026): [PDF no Drive](https://drive.google.com/file/d/1hklOLHgSxr0MH69i16Q9qJzhX6MihSFO/view)
- Gabarito definitivo de 2027: **ainda não publicado** em 08/11/2026.

## Conferências feitas em 08/11/2026

1. As letras de `gabarito_preliminar` nas 100 questões batem com o edital oficial.
2. Enunciados e alternativas foram comparados por trigramas com o texto do PDF da prova. Não há divergência de conteúdo, apenas diferenças de layout na tabela de densitometria da Q31.
3. Link do gabarito corrigido: o rascunho apontava para outro arquivo do Drive.
4. Segunda leitura clínica das 11 questões bloqueadas: ver [`revisao_questoes_bloqueadas.md`](revisao_questoes_bloqueadas.md).

## Arquivos

- [`justificativas_flashcards.md`](justificativas_flashcards.md): leitura completa (enunciado, gabarito, justificativa, alternativas, ressalvas, flashcard e referências).
- `Santa_Casa_2027_Justificativas_Flashcards_RASCUNHO.docx`: mesma versão em Word, para revisão.
- `Santa_Casa_2027_Leitura.html`: versão de leitura em navegador (usa a pasta `figuras/`).
- `editorial/questoes_editorial.csv`, `editorial/flashcards_editorial.csv`, `editorial/ressalvas.csv`: CSV em UTF-8, separador `;`. São arquivos para incorporação posterior; o formato não presume compatibilidade com o importador atual do MEDUNIDAVI.
- `figuras/`: figuras originais da prova (ECG da Q30 e forest plot da Q58).

## Padrão editorial (o mesmo do trabalho AMRIGS)

Gabarito com justificativa principal, comentário de cada alternativa e um flashcard autônomo quando útil. Quando o cartão seria ambíguo ou dependeria do contexto, a questão fica sem flashcard e a recomendação é reaplicá-la. Questões oficiais são preservadas sem alteração, mesmo quando têm defeitos; as ressalvas ficam explícitas. Bloqueios são decisões editoriais provisórias, não anulações da banca.

## Próximos passos

1. Curadoria docente das 11 questões bloqueadas (recomendações na revisão).
2. Quando o gabarito definitivo for publicado, conferir anulações e alterações (prioridade: Q28, Q35, Q38, Q52 e Q90).
3. Revisão humana amostral das 89 questões em `draft` antes de liberar ao estudante.
