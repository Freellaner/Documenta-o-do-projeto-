# 📘 Documentação da Plataforma Freellaner 
Esta documentação serve como guia essencial para entender a estrutura, o design e o funcionamento da plataforma Freellaner, focada em conectar freelancers e clientes.

# 1. 🚀 Visão Geral e Início Rápido
O projeto é um aplicativo web moderno, construído com React (a biblioteca principal para a interface).

Instalação e Funcionamento
Para colocar o projeto para rodar:

Instalação: Abra o terminal na pasta do projeto e execute npm install.

Execução: Execute npm run dev. O site estará acessível no seu navegador.

# ✨ Funcionalidades Destacadas
Identidade Visual Única: Design de alto contraste com a fonte Poppins e um sistema de temas Claro/Escuro (Dark/Light Mode) fácil de manter.

Gestão de Talentos: Telas dedicadas para buscar, ver detalhes de projetos e convidar freelancers (/dashboard/buscar-projetos, /dashboard/convidar-freelancer).

Transações: Tela de resumo financeiro com saldo e a funcionalidade de Saque (pop-up).

Segurança: A área principal (/dashboard) é totalmente protegida e só pode ser acessada por usuários autenticados.

# 2. 🗺️ Estrutura de Páginas e Navegação
Ótimo! Entendido. Vou refazer o item 2 da documentação, que trata da estrutura de rotas e páginas, organizando as informações em um formato de lista mais descritivo e direto, eliminando o visual de tabela.

2. 🗺️ Estrutura de Páginas e Navegação (Detalhada)
O aplicativo é estruturado em duas grandes áreas (Pública e Protegida) e usa o caminho /dashboard como a área restrita principal.

Páginas de Acesso Geral (Públicas)
Essas telas são acessíveis a qualquer visitante:

LandingPage (/): É a vitrine do seu negócio. Apresenta o produto, os benefícios e o design geral, direcionando o usuário para criar uma conta ou fazer login.

Login (/login): O portal de entrada para usuários já registrados.

Cadastro (/cadastro): Onde novos usuários criam sua conta na plataforma.

Termos de Serviço (/termos-de-servico): Documentação legal da plataforma, essencial para transparência.

Páginas Protegidas (Dashboard)
Todas as páginas abaixo são acessíveis apenas após o login, usando o prefixo /dashboard.

Páginas de Informação e Gerenciamento Pessoal
Dashboard (Rota Index): A primeira tela após o login. Apresenta um resumo executivo das atividades, saldo financeiro e tendências de ganhos.

Perfil (/dashboard/perfil): Onde o usuário pode ver e editar suas informações pessoais e profissionais, como habilidades e biografia.

Transacoes (/dashboard/transacoes): Gerenciamento e visualização do histórico de pagamentos, recebimentos e saldo para solicitações de saque.

Relatorios (/dashboard/relatorios): Seção de métricas e dados analíticos sobre o desempenho do usuário ou dos projetos.

Páginas de Mercado (Ação e Detalhes)
Buscar Projetos (/dashboard/buscar-projetos): Para o freelancer, é a lista principal para encontrar e filtrar oportunidades de trabalho disponíveis.

Encontrar Freelancers (/dashboard/encontrar-freelancers): Para o cliente, é o catálogo de talentos para buscar o profissional ideal.

Página de Detalhes de projetos (/dashboard/projeto/:id): Onde o usuário visualiza todos os detalhes, requisitos e descrição de um projeto antes de se candidatar.

Pagina de Convite de Freelancers (/dashboard/convidar-freelancer/:freelancerId): O formulário que o cliente usa para enviar um convite personalizado a um talento específico.

PaginaProposta (/dashboard/pagina-proposta): O formulário detalhado que o freelancer usa para criar e enviar uma proposta formal.
# 3. 🎨 Manutenção e Design
O design é baseado em regras CSS simples e reutilizáveis para garantir a consistência e a facilidade de manutenção.

# A. Cores e Temas
O projeto usa Variáveis CSS (nomes como --cor-primaria) para gerenciar a paleta de cores.

Cor Primária: O Azul Vibrante (--cor-primaria) é usado para os botões de ação (CTAs), títulos importantes e ícones, sendo o centro da identidade visual.

Temas (Dark/Light): Ao mudar o tema, apenas as variáveis de fundo e texto são trocadas, garantindo que o design permaneça idêntico, apenas com cores invertidas.

# B. Elementos de UI (User Interface)
Cards Flutuantes: A maioria dos cartões (vagas, depoimentos) usa a mesma cor do fundo da página. O destaque e a separação são feitos com bordas finas e sombras suaves, dando um efeito sofisticado e menos pesado.

Animações: As telas de apresentação usam a biblioteca Framer Motion para criar transições suaves e o efeito de "aparecer na rolagem", tornando a experiência mais moderna.

Botões de Ação: São o ponto focal. Usam gradientes de cor e têm um estado de :hover que faz o botão se elevar e brilhar, incentivando o clique.

# C. Manutenção de Código (Regra de Ouro)
Consistência de Nomes: Ao criar uma nova página, o nome do arquivo (NomeDoArquivo.jsx) e o nome da função do componente (const NomeDoArquivo = () => ...) devem sempre começar com letras maiúsculas.

Variáveis de Cor: Para mudar qualquer cor no site, modifique apenas as variáveis na seção :root do CSS. Nunca use cores hexadecimais diretamente nos elementos.
