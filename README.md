# Projeto: Cordel Moderno (clonagem)

Breve documentação do projeto criado para reproduzir a página "Cordel Moderno" do Professor Guanabara.

Propósito
- Reproduzir localmente o layout e conteúdo do exemplo "Projeto Cordel" para estudo e prática de HTML/CSS.

Conteúdo do repositório
- `index.html` — página principal com o poema e créditos.
- `style.css` — estilos aplicados para tipografia, fundo e layout (contém import da fonte `Italianno`).

Como abrir / testar localmente
1. Abra o `index.html` diretamente no navegador (duplo-clique). Note que em alguns navegadores o carregamento de recursos pode ser bloqueado quando aberto via `file://`.
2. Recomendado: iniciar um servidor local para evitar problemas de cache e CORS. No PowerShell execute no diretório do projeto:

```powershell
cd 'c:\Users\local\do\seu\projeto'
python -m http.server 8000; Start-Process http://localhost:8000
```

3. No Chrome, para forçar atualização do CSS use DevTools → Network → marque "Disable cache" e recarregue, ou use "Empty Cache and Hard Reload".

Fonte
- A fonte usada nas estrofes é `Italianno` (Google Fonts). O `style.css` importa a fonte via:

```css
@import url('https://fonts.googleapis.com/css2?family=Italianno&display=swap');
```

- Caso prefira usar a fonte localmente (offline), adicione os arquivos `.woff`/`.woff2` em `fontes/` e registre-os via `@font-face` no `style.css`.

Créditos
- Conteúdo original do poema: Milton Duarte (link no `index.html`).
- Exemplo original: Gustavo Guanabara — Projeto de demonstração.

Licença e notas
- Este repositório é apenas uma cópia para fins de estudo e prática. Verifique as licenças de fontes/imagens antes de publicar.
- O arquivo `fontes/OFL.txt` contém a licença Open Font License (se aplicável) para as fontes.

Próximos passos sugeridos
- Baixar os assets (favicon e imagens usadas no original) para `imagens/`.
- Ajustar estilos finos para ficar idêntico ao original (espessuras, espaçamentos, fontes alternativas).
- Testar em diferentes tamanhos de tela e navegadores.
