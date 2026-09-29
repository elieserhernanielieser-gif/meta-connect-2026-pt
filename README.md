# Meta Connect 2026 – Keynote legendado em português

Página web com o keynote de Mark Zuckerberg no **Meta Connect 2026** legendado em português. As legendas foram traduzidas manualmente a partir do inglês.

A página tem duas versões do vídeo:

- **Versão legendada:** vídeo local, com legendas em português (WebVTT).
- **Versão original:** vídeo incorporado do YouTube (iframe), com link para ver no próprio YouTube.

**Vídeo original:** [LIVE: Mark Zuckerberg's Meta Connect 2026 keynote](https://youtu.be/hI3M_4UQoWk)

## Funcionalidades

- Vídeo local com legendas em português (`<track>` + WebVTT)
- Vídeo original incorporado via iframe do YouTube
- Link para a página original do vídeo no YouTube
- Secção com resumo e destaques do keynote
- Layout responsivo com tema escuro

## Tecnologias

- HTML5
- CSS3
- JavaScript (vanilla)
- WebVTT

## Estrutura do projeto

```
meta-connect-2026-pt/
├── index.html
├── assets/
│   ├── images/
│   ├── icons/
│   └── videos/
├── css/
│   └── style.css
├── js/
│   └── main.js
├── subtitles/
│   └── pt.vtt
└── README.md
```

## Como executar

1. Clona o repositório:

   ```bash
   git clone https://github.com/elieserhernanielieser-gif/meta-connect-2026-pt.git
   cd meta-connect-2026-pt
   ```

2. Abre a pasta no VS Code ou um outro editor de código.

3. Com a extensão Live Server instalada, clica com o botão direito em **index.html** e escolhe Open with Live Server (ou clica em Go Live na barra inferior). O servidor local é necessário para o browser carregar o ficheiro **.vtt**.

## Como funcionam as legendas

O ficheiro `subtitles/pt.vtt` contém as legendas em português no formato WebVTT, com o tempo de início e fim de cada linha. O vídeo local carrega-o com a tag `<track>`:

```html
<video controls>
  <source src="assets/videos/keynote.mp4" type="video/mp4">
  <track label="Português" src="subtitles/pt.vtt" kind="subtitles" srclang="pt-pt" default>
</video>
```

Exemplo do formato do ficheiro:

```
WEBVTT

00:00:01.000 --> 00:00:04.000
Olá a todos, bem-vindos ao keynote.
```

## Créditos

- Vídeo e conteúdo original: Meta, através do canal oficial no YouTube.
- Tradução das legendas para português, design e desenvolvimento: **Elieser Hernani**.

## Licença

O código deste repositório está sob a licença [MIT](LICENSE). A licença não cobre o vídeo nem o seu conteúdo, que pertencem aos respetivos autores.
