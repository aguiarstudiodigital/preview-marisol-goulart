# Marisol Goulart — V3.5 | Publicação e SEO/GEO

## Alteração da V3.5
- Cabeçalho: imagem original de baixa resolução substituída por monograma branco em PNG transparente de resolução maior, reconstruído a partir da referência visual aprovada. O nome permanece como texto HTML, garantindo nitidez e legibilidade.
- Retirado o círculo colorido do Instagram, que não faz parte da marca.
- Favicon simplificado sem anel colorido; novas aplicações em `assets/marisol-monograma-branco.png`, `assets/marisol-monograma-escuro.png` e `assets/marisol-logo-completa-branca.png`.
- A reconstrução é uma aproximação visual, não uma vetorização exata da marca original.

## O que foi implementado
- Política de Privacidade e Termos de Uso em páginas HTML independentes, links no rodapé e consentimento do formulário.
- Informações sobre cookies e serviços externos integradas à Política de Privacidade. Não há banner de cookies: não foram identificados rastreadores de marketing no código atual.
- Metadados Open Graph, Twitter Card, ícone, descrição, estrutura HTML e JSON-LD (`Person` e `WebSite`).
- `noindex,follow` nas três páginas durante a fase de prévia do GitHub Pages. `robots.txt` permite acesso para que os buscadores leiam a diretiva `noindex`.
- Não há sitemap da prévia, pois deliberadamente não desejamos indexá-la. Sitemap XML deve ser gerado com o domínio final.
- Fotos, vídeos, paleta, menu, seções e funcionalidades principais mantidos.

## Antes de subir ao GitHub
1. Verificar se a fotografia editorial gerada em Moda & Compras foi aprovada; não a apresentar como fotografia real da Marisol.
2. Validar com Marisol a identidade do controlador LGPD, política de retenção, destinatário do formulário e texto legal. As páginas são minutas operacionais, não parecer jurídico.
3. Subir `index.html`, `politica-de-privacidade.html`, `termos-de-uso.html`, `robots.txt`, pastas `assets/`, `css/`, `js/`. Evitar publicar versões anteriores, documentos internos e arquivos de teste.
4. Confirmar que as páginas legais abrem e que o menu, vídeos, fotos e links funcionam.
5. Ativar e validar FormSubmit no e-mail `contato@aguiarstudiodigital.com` com submissão real e confirmação na caixa de entrada; resposta de API não comprova entrega.

## Quando migrar para domínio oficial (HostGator) — CHECKLIST OBRIGATÓRIO
1. Definir o domínio canônico, com ou sem `www`, e configurar HTTPS.
2. REMOVER `<meta name="robots" content="noindex,follow,max-image-preview:large">` e `<meta name="googlebot" content="noindex,follow">` da home, e `<meta name="robots" content="noindex,follow">` das páginas legais. Alternativamente, definir `index,follow`.
3. Adicionar `<link rel="canonical" href="https://DOMINIO-OFICIAL/">` à home e URLs canônicas específicas às páginas legais, com URLs reais.
4. Substituir todas as URLs `https://aguiarstudiodigital.github.io/preview-marisol-goulart/` em `index.html` (metas OG e JSON-LD) pelo domínio oficial. Atualizar imagens OG e eventuais links absolutos.
5. Criar `sitemap.xml` válido com URLs HTTPS absolutas das páginas indexáveis (pelo menos home; páginas legais se desejar indexá-las), hospedado na raiz; adicionar `Sitemap: https://DOMINIO-OFICIAL/sitemap.xml` em `robots.txt`.
6. Confirmar responsável LGPD, e-mail de contato, política de retenção, termos, FormSubmit, consentimento e eventual uso de cookies/GA4/Meta Pixel. Não ativar tags não essenciais sem avaliação e consentimento aplicável.
7. Configurar e verificar a propriedade do domínio no Google Search Console, enviar sitemap, inspecionar URL da home e acompanhar cobertura/indexação. Não garantir indexação ou citações por IA.
8. Validar performance e acessibilidade em desktop/mobile, inclusive vídeos, navegação, formulários, Open Graph, status HTTP e dados estruturados.
9. Somente DEPOIS de validar o domínio definitivo, desativar o GitHub Pages; manter o repositório como histórico, se desejar.

## GEO
O JSON-LD descreve apenas fatos confirmados e o conteúdo textual apresenta claramente os projetos. Não existe garantia de aparição em respostas de IA. Reavaliar `sameAs`, marca, contatos e perfis oficiais no lançamento.

## Status dos testes
- Sintaxe do JavaScript e integridade dos arquivos: verificadas automaticamente.
- Entrega de e-mails: NÃO testada (requer confirmação do destinatário).
- Auditoria visual real no celular e desempenho em rede: pendentes.
- Publicação GitHub/HostGator: NÃO realizada.
