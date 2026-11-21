# Roteiro do Projeto (seu guia de estudo)

Cada etapa abaixo é o que acontece num projeto real. Marque conforme avançar.
**Combinado:** você faz, me mostra o que fez, e eu corrijo e explico. Não pule etapas.

| # | Etapa | O que você aprende | Status |
|---|---|---|---|
| 0 | Preparar ambiente (Git, Python, estrutura de pastas) | Reprodutibilidade, versionamento | [ ] |
| 1 | Entender o negócio e o briefing | Traduzir pergunta de negócio em pergunta de dados | [ ] |
| 2 | Explorar os dados (EDA inicial) | Ler dados, tipos, tamanho, nulos | [ ] |
| 3 | Dicionário de dados e auditoria de qualidade | Documentar problemas antes de corrigir | [ ] |
| 4 | Limpeza e tratamento (script reproduzível) | Pandas, decisões justificadas | [ ] |
| 5 | Modelagem em banco de dados (SQLite) | Chaves, relacionamentos, carga | [ ] |
| 6 | Análises em SQL | JOIN, GROUP BY, CTE, window functions | [ ] |
| 7 | Análises e gráficos em Python | Storytelling com dados | [ ] |
| 8 | (Opcional) Dashboard | Power BI ou Streamlit | [ ] |
| 9 | Relatório executivo | Comunicar para não técnicos | [ ] |
| 10 | Polimento do GitHub | README, commits, portfólio | [ ] |

## Regras de ouro (o que diferencia amador de profissional)

1. **Nunca edite os dados brutos.** `data/raw/` é somente leitura. Todo tratamento vira código.
2. **Tudo reproduzível.** Alguém clona o repositório e chega no mesmo resultado.
3. **Documente decisões.** "Removi X porque Y" vale mais que o código.
4. **Commits pequenos e com mensagem clara** (ex.: `Adiciona auditoria de nulos em clientes`).
5. **Valide seus números.** Se o total não bate, algo está errado antes de qualquer gráfico.
