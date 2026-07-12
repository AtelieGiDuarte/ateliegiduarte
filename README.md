# Sala de Exibição · Ateliê Gi Duarte

Site estático que mostra vídeos com descrição. Roda no GitHub Pages, sem servidor e sem custo.

## Endereço final

```
https://SEU-USUARIO.github.io/ateliegiduarte/
```

É esse o link que você manda pra pessoa assistir.

---

## Passo a passo (primeira vez)

### 1. Crie o repositório

Em https://github.com/new:

- **Repository name:** `ateliegiduarte`
- **Public** (o Pages gratuito exige público)
- Não marque nada em "Initialize" — pode deixar limpo
- **Create repository**

### 2. Monte o `videos.json`

Abra o `estudio.html` no navegador (duplo clique no arquivo, aqui do seu computador mesmo).

1. Arraste os vídeos pra dentro.
2. Clique em **Editar** em cada card e escreva o título e a descrição.
3. Clique em **Baixar videos.json**.
4. Substitua o `videos.json` desta pasta pelo que você baixou.

O estúdio **não sobe nada** — ele só lê os vídeos pra pegar a duração e gerar o arquivo de configuração. Os vídeos não saem da sua máquina.

### 3. Copie os vídeos pra dentro da pasta `videos/`

Use exatamente o nome que aparece no card do estúdio (ele tira acentos e espaços, que o GitHub não engole bem). Exemplo: `Casamento Ana & João.mp4` vira `casamento-ana-joao.mp4`.

### 4. Suba tudo

Na página do repositório: **Add file → Upload files**, arraste estes arquivos e pastas:

```
index.html
estudio.html
estilo.css
videos.json
videos/          ← com os vídeos dentro
```

Clique em **Commit changes**.

### 5. Ligue o GitHub Pages

**Settings → Pages → Build and deployment**

- Source: **Deploy from a branch**
- Branch: **main** / pasta **/ (root)** → **Save**

Espere de 1 a 3 minutos. O link aparece nessa mesma tela.

---

## Pra adicionar vídeos depois

1. Abra o `estudio.html`, arraste **todos** os vídeos (os antigos e os novos), escreva as descrições, baixe o `videos.json` novo.
2. No repositório, suba os vídeos novos em `videos/` e substitua o `videos.json`.

Pronto — o site atualiza sozinho em poucos minutos.

## Truque: link direto pra um vídeo

Somando `#v2` no fim do endereço, a página já abre no segundo vídeo da lista:

```
https://SEU-USUARIO.github.io/ateliegiduarte/#v2
```

---

## Limites do GitHub Pages (respeite ou o vídeo não sobe)

| Limite | Valor |
|---|---|
| Tamanho de cada arquivo | **100 MB** (acima disso, o GitHub recusa) |
| Tamanho total do site | **1 GB** |
| Tráfego por mês | **100 GB** (limite flexível) |

Vídeo longo em alta qualidade estoura fácil os 100 MB. Antes de subir, exporte em H.264, 1080p, com bitrate por volta de 3–5 Mbps — dá uns 25–40 MB por minuto de vídeo. Se ainda assim passar, o caminho é hospedar o vídeo no Vimeo/YouTube não listado e usar o site só como vitrine.

## Uma coisa importante sobre privacidade

O repositório é público e o site também. Quem tiver o link, assiste — e quem souber o endereço do arquivo, baixa. Não coloque aqui material que não pode circular.
