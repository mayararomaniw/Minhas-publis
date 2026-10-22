# Minhas Publis — Controle financeiro

Aplicativo web responsivo/PWA para organizar publis e pagamentos.

## Arquivos
- `index.html`: aplicativo
- `manifest.json`: metadados de instalação
- `sw.js`: cache offline básico
- `icon-192.png` e `icon-512.png`: ícones

## Dados e privacidade
Os dados são guardados no `localStorage` do navegador do aparelho. Eles não são enviados a um servidor e não sincronizam entre aparelhos. Use **Exportar backup** para baixar um arquivo JSON e guardá-lo no Arquivos/iCloud Drive. Faça backup antes de limpar dados do navegador ou trocar de aparelho. A restauração substitui os dados atuais.

## Publicação grátis
Hospede todos os arquivos preservando a estrutura em um serviço de hospedagem estática HTTPS, por exemplo Netlify Drop (https://app.netlify.com/drop) ou GitHub Pages. Após publicar, teste o endereço em uma aba do Safari. Não renomeie `index.html`, `manifest.json`, `sw.js` nem os ícones. Para instalar no iPhone, abra o link no Safari > Compartilhar > Adicionar à Tela de Início.

## Limitação importante
Este pacote não configura sincronização em nuvem. Para dados sincronizados e recuperação automática entre aparelhos, será necessário integrar um serviço de banco de dados com autenticação e regras de segurança (por exemplo Supabase). Não guarde informações bancárias sensíveis neste app.
