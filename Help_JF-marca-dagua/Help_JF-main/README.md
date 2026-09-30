# Marca d'Água

Site estático de conscientização sobre desastres naturais no Brasil — o que aconteceu
entre 2022 e 2026, o tamanho do problema em números oficiais e como ajudar quem foi atingido.

## Estrutura

```
index.html   páginação completa (uma página) + script de animação (~30 linhas, sem dependências)
index.css    sistema visual: tokens, componentes, animações e responsividade
img_logo/    logo do site e logos dos veículos de imprensa
```

Sem build, sem framework, sem pacote. Abrir o `index.html` no navegador já funciona,
e o deploy no GitHub Pages é direto.

## Seções

| Seção | Conteúdo |
| --- | --- |
| Hero | Régua fluviométrica com os níveis e volumes recordes de cada desastre |
| Panorama | Números de 2025 do Cemaden, com contagem animada |
| Registros | Cinco desastres em ordem cronológica, cada um com seu medidor |
| Como ajudar | Doação financeira, materiais e trabalho voluntário |
| Prevenção | O que fazer antes, durante e depois |
| Notícias | Veículos com cobertura contínua |

## Design

- **Paleta** — papel `#F1F5F6`, fundo profundo `#0C2B33`, água `#128C9E`; um único acento
  quente `#D9533C`, reservado às marcas de nível.
- **Tipografia** — Bricolage Grotesque (display), Instrument Sans (texto), JetBrains Mono (dados).
- **Movimento** — entrada escalonada no hero, revelação por `IntersectionObserver`,
  medidores que enchem (ou esvaziam, no caso da seca) e transições de cortina nos botões.
  Tudo desligado sob `prefers-reduced-motion`.

## Fontes dos dados

- [Cemaden — Estado do Clima, Extremos de Clima e Desastres no Brasil (2025)](https://www.gov.br/cemaden/pt-br)
- [Agência Brasil — balanço de desastres climáticos de 2025](https://agenciabrasil.ebc.com.br/meio-ambiente/noticia/2026-02/desastres-climaticos-afetaram-mais-de-336-mil-pessoas-no-pais-em-2025)
- [Serviço Geológico do Brasil — níveis de rios e cotas históricas](https://www.sgb.gov.br/)
- [Defesa Civil Nacional](https://www.gov.br/defesacivil/)

---

Desenvolvido por Markos Samuell · Senai CTTI-MG
