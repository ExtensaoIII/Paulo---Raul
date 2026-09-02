<img width="1903" height="938" alt="image" src="https://github.com/user-attachments/assets/170a542f-a9d7-4141-82fd-37e0df847b78" />

# EcoPilha — protótipo

Protótipo estático de um site/app para reciclagem de pilhas e baterias, com mapa de pontos de coleta, gamificação por peso reciclado e parcerias com o comércio local. Construído apenas com **HTML e CSS** (sem JavaScript, sem dependências de build).

## Arquivos

```
ecopilha-prototipo.html   → página única com todo o HTML e CSS embutido
README.md                 → este arquivo
```

## Como visualizar

Basta abrir `ecopilha-prototipo.html` diretamente no navegador (duplo clique ou arrastar para uma aba). Não precisa de servidor local nem instalação.

## O que está no protótipo

- **Cabeçalho fixo** com navegação e chamada para ação
- **Hero** com um medidor de carga animado (progresso do mês em kg)
- **Barra de estatísticas** gerais do programa
- **Seção educativa** sobre o impacto do descarte incorreto
- **Como funciona** — 4 passos, com um mapa de pontos de coleta simulado em CSS (ruas, quarteirões e pinos)
- **Recompensas** — escada de níveis por quilo reciclado (Semente → Carga plena) e um cartão de certificado ambiental
- **Comércio parceiro** — cartões de desconto local
- **Impacto / ODS** — selos próprios (não são os ícones oficiais da ONU) para os Objetivos 11, 12, 13 e 15
- **Faixa de CTA** com formulário de espera (e-mail + CEP)
- **Rodapé** com navegação secundária

Todos os dados (estatísticas, parceiros, certificado) são fictícios, só para ilustrar o conceito.

## Personalizar

Tudo fica em um único arquivo, dentro da tag `<style>`:

| O que mudar | Onde procurar |
|---|---|
| Cores | bloco `:root` no topo do CSS (`--ink`, `--paper`, `--volt`, `--moss`, `--rust`) |
| Fontes | `<link>` do Google Fonts no `<head>` + `font-family` em `body`/`h1,h2,h3` |
| Textos | diretamente no HTML de cada `<section>` |
| Nome da marca | busque por "EcoPilha" no arquivo (aparece na logo, título, certificado, rodapé e e-mail) |

## Responsividade

O layout se adapta em três larguras: acima de 920px (desktop), até 920px (tablet) e até 560px (celular), via `@media queries` no fim do CSS.

## Tecnologias

- HTML5
- CSS3 (Flexbox, Grid, `@keyframes`, `clamp()`, `prefers-reduced-motion`)
- Fontes: Archivo (títulos) e Public Sans (texto), via Google Fonts
