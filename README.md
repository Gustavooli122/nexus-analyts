# Nexus Analytics

**Dashboard administrativo responsivo para projetos SaaS, lojas e sistemas de gestão.**

O **Nexus Analytics** é um template de front-end desenvolvido com HTML5, Tailwind CSS e JavaScript puro. Ele reúne indicadores, gráficos interativos e telas de gerenciamento em uma interface moderna, com temas claro e escuro. O projeto usa **dados fictícios**, para demonstração e personalização.



## Funcionalidades

- **Dashboard:** indicadores de receita, pedidos, novos clientes e taxa de conversão; gráficos de receita e vendas; pedidos recentes; produtos mais vendidos e atividades simuladas.
- **Analytics:** gráficos interativos, origem do tráfego e indicadores de desempenho.
- **Pedidos:** tabela com busca, filtro por status, ordenação, paginação e exportação CSV.
- **Produtos:** catálogo com busca e formulários para adicionar, editar e excluir produtos.
- **Clientes:** listagem com pesquisa por nome ou e-mail e informações de compras.
- **Relatórios:** resumo de indicadores, visualizações gráficas e exportação em CSV.
- **Configurações:** edição do perfil demonstrativo, preferências de visualização, notificações e troca entre tema claro e escuro.
- **Layout responsivo:** navegação adaptada para desktop, tablet e celular.

## Tecnologias

| Tecnologia | Uso |
| --- | --- |
| HTML5 | Estrutura da interface |
| Tailwind CSS (CDN) | Estilização e responsividade |
| JavaScript (Vanilla JS) | Navegação, formulários, filtros e interações |
| Chart.js (CDN) | Gráficos interativos |
| Lucide Icons (CDN) | Ícones |
| Google Fonts — Inter | Tipografia |
| `localStorage` | Armazenamento local do catálogo de produtos, perfil e preferências |

**Não é necessário instalar Node.js, React ou dependências para visualizar a demonstração.**

## Como executar

1. Extraia os arquivos do pacote adquirido.
2. Localize o arquivo HTML principal (`index.html` ou `dashboard.html`, conforme o nome recebido).
3. Abra o arquivo no navegador ou utilize a extensão **Live Server** do VS Code.
4. Mantenha uma conexão com a internet para carregar Tailwind CSS, Chart.js, Lucide e a fonte Inter pelos CDNs.

### Publicação no GitHub Pages

1. Crie um repositório no GitHub e envie os arquivos do projeto.
2. Deixe o arquivo principal com o nome **`index.html`** na raiz do repositório.
3. Acesse **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**, sua branch de publicação (por exemplo, `main`) e a pasta **`/(root)`**.
5. Salve e acompanhe o processo na aba **Actions**.

Para hospedar sob outro nome de arquivo, como `dashboard.html`, inclua esse nome no final do endereço do site.

## Personalização

O template foi organizado em um único arquivo HTML, com os estilos adicionais e o JavaScript necessários para a demonstração. Você pode editar:

- **Cores e tipografia:** configurações do Tailwind no `<head>` e classes aplicadas aos elementos.
- **Produtos de exemplo:** array `seedProducts` no JavaScript.
- **Clientes e pedidos demonstrativos:** dados e geradores de exemplo definidos no script.
- **Indicadores e gráficos:** funções `metrics()`, `timeline()` e `initPageCharts()`.
- **Seções do painel:** funções de renderização e objeto `pageTitles`.

> Para usar o painel com dados reais, será necessário integrá-lo ao seu próprio backend ou API, incluindo autenticação, persistência no servidor e regras de negócio.

## Observações importantes

Este é um **template demonstrativo de front-end**, não um sistema SaaS pronto para produção:

- Os números, clientes, pedidos, atividades e notificações exibidos são **fictícios**.
- Não há backend, banco de dados, autenticação real nem processamento de pagamentos.
- Os dados locais do catálogo, as preferências e as informações de perfil são salvos no **navegador atual** por meio do `localStorage`; não são sincronizados entre dispositivos.
- A exportação CSV é gerada localmente no navegador.
- O uso de bibliotecas por CDN requer acesso à internet. Antes de usar o projeto em produção, revise o carregamento das dependências e os requisitos de segurança e desempenho.

## Licença e suporte

**Licença de uso:** consulte os termos informados na página de venda ou no arquivo `LICENSE`, caso acompanhe o pacote. Não presuma direitos de redistribuição ou revenda do código sem autorização explícita.

**Suporte:** consulte os canais e condições informados na página do produto.

---

**Nexus Analytics** — um ponto de partida personalizável para interfaces administrativas modernas.
