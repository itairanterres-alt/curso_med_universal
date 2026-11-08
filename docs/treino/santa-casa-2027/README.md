# Santa Casa/UFCSPA 2027 — Acesso Direto: material para o treino MEDUNIDAVI

**Situação:** RASCUNHO EDITORIAL, sem liberação ao estudante (`student_visible = false`).

Resolução própria das 100 questões a partir do PDF da prova, com justificativa, comentário de cada alternativa, flashcard e ressalvas, seguida de confronto com o gabarito e auditoria cruzada com a V2 produzida pelo ChatGPT. O método, os limites e os resultados estão em [`AUDITORIA.md`](AUDITORIA.md).

| Indicador | Valor |
|---|---|
| Questões comentadas (justificativa + A–D) | 100 |
| Flashcards | 95 |
| Concordância com o gabarito preliminar | 95/100 (resolução **não cega**) |
| Bloqueadas até o gabarito definitivo | 28, 38, 52, 88, 90 |
| Divergências com a V2 do ChatGPT, para decisão do curador | 33, 35, 58, 86, 100 |

## Fontes
- Prova: [UFCSPA-Medica-ACESSO-DIRETO.pdf](https://drive.google.com/file/d/184wAibaUuAJcpkbtZ278HfPk7dmhIqAf/view)
- Gabarito **preliminar** (Edital nº 06, 04/11/2026): [FUNDMED](https://fundmed.org.br/website/wp-content/uploads/2026/08/UFCSPA-MEDICA-Gabarito-preliminar-e-disponibilizacao-do-resultado-preliminar-da-prova-objetiva.pdf). As cópias no Drive são idênticas.
- Gabarito definitivo de 2027: ainda não publicado em 08/11/2026.
- V2 do ChatGPT, usada só na auditoria: `Santa_Casa_2027_Medunidavi_V2_RASCUNHO.zip`, no Drive.

## Arquivos
- [`Santa_Casa_2027_Claude_Justificativas_Flashcards.md`](Santa_Casa_2027_Claude_Justificativas_Flashcards.md) e a versão `.docx`: documento de leitura completo, com as figuras da Q30 e da Q58.
- [`AUDITORIA.md`](AUDITORIA.md): método, limites, divergências com o gabarito e com a V2, e autocrítica.
- `claude/bloco_*.md`: texto-fonte por área (cirurgia, clínica, preventiva/MFC, GO, pediatria).
- `claude/questoes_claude.csv`: uma linha por questão, com resposta, confiança, gabarito, justificativa, comentários A–D, flashcard, ressalva, status e as decisões da V2 para comparação. UTF-8, separador `;`.
- `claude/flashcards_claude.csv`: 95 cartões.
- `figuras/`: ECG da Q30 e forest plot da Q58.

O pacote é editorial e não é um lote nativo do importador do MEDUNIDAVI.
