# Apresentações em PDF — Segurança da Informação

Versões em PDF dos três decks apresentados na Martha Falcão Wyden (Prof. Ranyere Lima).

**Página de download:** https://cauelimsia.github.io/apresentacoes-pdf/

| Arquivo | Disciplina | Páginas |
|---|---|---|
| `Classificacao-e-Descarte.pdf` | Introdução à Segurança da Informação | 31 |
| `Resumo-Tema-1-Seguranca-da-Informacao.pdf` | Introdução à Segurança da Informação | 19 |
| `Simulado-ENADE-Seguranca-da-Informacao.pdf` | Introdução à Segurança da Informação | 6 |
| `Dentro-da-Maquina.pdf` | Introdução à Segurança da Informação | 43 |
| `Falhar-com-Seguranca.pdf` | Desenvolvimento de Software Seguro | 9 |

## Por que mais páginas do que slides

Os decks revelam conteúdo aos poucos: o veredito do quiz, o gabarito do simulado, a
simulação do fail-safe. O PDF foi gerado dirigindo a própria navegação do deck
(`DECK.proximo()`) num Chromium headless e fotografando a tela a cada mudança — então cada
revelação virou uma página, na mesma ordem em que aparece na aula. Daí 18 slides virarem
31 páginas.

Os decks em si não foram alterados para a exportação; o único ajuste vive no script de
captura, que desliga as animações de entrada, o cartão do código do controle remoto e a
camada de grão de filme (ruído por pixel, que sozinho levava um dos PDFs a 132 MB).

## O resumo do Tema 1

`Resumo-Tema-1-Seguranca-da-Informacao.pdf` não vem de deck nem do SAVA: o HTML é escrito
no próprio script de geração e impresso em páginas de 1280x720, uma por slide. O script mede
`scrollHeight` contra `clientHeight` de cada slide antes de imprimir, porque em formato 16:9
texto que passa da altura some sem erro nenhum.

## O simulado em documento

`Simulado-ENADE-Seguranca-da-Informacao.pdf` não é uma exportação de slides: o script lê o
array `QUESTOES` do próprio deck dentro do navegador e formata em A4 corrido. O texto não é
copiado, então documento e apresentação não têm como divergir — e, fora do slide, a resposta
não precisa caber em 768px de altura.

## Versão interativa

- https://cauelimsia.github.io/classificacao-descarte-apresentacao/
- https://cauelimsia.github.io/hardware-so-iso-apresentacao/
- https://cauelimsia.github.io/software-seguro-apresentacao/
