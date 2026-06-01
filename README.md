# Sala de Prova IDIB — Técnico I · Enfermeiro (Araguaína-TO)

Simulado de questões no padrão IDIB para o cargo de **Técnico I – Enfermeiro** do
Concurso Público **001/2026** da Prefeitura Municipal de Araguaína-TO.

- Banco curado de questões, restrito ao **Anexo III** do edital.
- 4 alternativas (A–D), foco em aplicação clínica e de gestão (item 18.5).
- **Não repete** questões já respondidas (memória salva no navegador).
- Três modos (misto / específicos+SUS / só específicos), 5 a 20 questões, três níveis.
- Funciona **offline** e pode ser **instalado** na tela inicial do celular.

É um site estático (um único `index.html`), então roda direto no **GitHub Pages**, sem servidor.

---

## Arquivos do repositório

| Arquivo | Função |
|---|---|
| `index.html` | O aplicativo completo |
| `manifest.webmanifest` | Permite instalar como app no celular |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | Ícones do app |
| `.nojekyll` | Faz o GitHub Pages servir os arquivos sem processamento |
| `README.md` | Este arquivo |

> Mantenha todos os arquivos na **raiz** do repositório (mesma pasta do `index.html`).

---

## Publicar no GitHub Pages — pelo navegador (ideal no celular)

1. Acesse **github.com**, toque em **+** → **New repository**.
2. Nome sugerido: `simulado-idib-enfermeiro`. Marque **Public**. Crie o repositório.
3. Na página do repositório vazio: **Add file → Upload files**.
4. Envie **todos** os arquivos desta pasta (incluindo os `.png` e o `.nojekyll`).
   Toque em **Commit changes**.
5. Abra **Settings → Pages** (menu do repositório).
6. Em **Build and deployment → Source**, escolha **Deploy from a branch**.
7. Em **Branch**, selecione **main** e a pasta **/ (root)**. Toque em **Save**.
8. Aguarde ~1 minuto e recarregue a página de Pages. Seu link público aparecerá:

   ```
   https://SEU-USUARIO.github.io/simulado-idib-enfermeiro/
   ```

Pronto — esse link funciona em qualquer celular ou computador.

---

## Publicar via Git (computador)

```bash
git init
git add .
git commit -m "Sala de Prova IDIB - Enfermeiro"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/simulado-idib-enfermeiro.git
git push -u origin main
```

Depois ative o **GitHub Pages** em **Settings → Pages** (branch `main`, pasta `/root`).

---

## Instalar como app no celular

- **iPhone (Safari):** abra o link → botão Compartilhar → **Adicionar à Tela de Início**.
- **Android (Chrome):** abra o link → menu (⋮) → **Instalar app** / **Adicionar à tela inicial**.

---

## Observações

- A memória de "não repetir" e as estatísticas ficam salvas **no navegador de cada
  pessoa** (armazenamento local). Limpar os dados do navegador zera o progresso;
  o app também tem o botão **"Zerar progresso"** no rodapé.
- O banco de questões é finito. Para **geração de questões ao vivo e ilimitada por IA**
  (sem repetição compartilhada entre dispositivos), é necessária uma versão com
  back-end e banco de dados — por exemplo na plataforma Base44, usando a função
  `InvokeLLM` e uma entidade para registrar as questões já usadas.
