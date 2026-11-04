Descubra Nossa Cidade

Portal turístico criado para reunir, em um único lugar, informações sobre atrações, eventos, lazer, gastronomia, comércio local e canais públicos de uma cidade.

Situação da stack: a interface inicial foi criada em React com Vite. Para implementar cadastro, login, recuperação de senha, área restrita, persistência de usuários e envio de e-mails, o projeto foi migrado para React com Next.js e Payload CMS dentro do Figma Make. O histórico anterior à migração permanece registrado no Git.

Problema

Informações turísticas municipais normalmente ficam distribuídas entre redes sociais, páginas institucionais e divulgações isoladas. Isso dificulta que moradores e visitantes encontrem eventos, atrações, serviços e contatos confiáveis.

Objetivo

Oferecer um portal responsivo e acessível que:

apresente os principais atrativos da cidade;
concentre notícias, festas, eventos e atividades de lazer;
facilite o planejamento de visitas;
aproxime visitantes, comerciantes, organizadores e prefeitura;
permita que usuários criem uma conta e mantenham um histórico de navegação.

Funcionalidades

Portal público

Página inicial responsiva;
navegação para atrações, agenda, planejamento e prefeitura;
carrossel de eventos e atividades;
categorias de cultura, natureza, gastronomia e festas;
atalhos para hospedagem, alimentação, comércio e transporte;
contatos da prefeitura e da Secretaria de Turismo;
espaços destinados a vendedores e organizadores de eventos.

Autenticação

Cadastro de usuário;
login por e-mail e senha;
recuperação de senha por e-mail;
redefinição de senha por link temporário;
área restrita;
proteção de rotas;
logoff seguro;
bloqueio temporário após várias tentativas incorretas.

Tecnologias

React 19;
TypeScript;
Next.js App Router;
Payload CMS;
Tailwind CSS 4;
Resend para recuperação de senha por e-mail;
pnpm;
Figma Make;
Git e GitHub.

Integrantes:

Gedson Eber Ribeiro Silva 
(01770703)

Julio Ferreira da Silva Neto 
(01808964)

Iarlley Oliveira França 
(01812784)

Wendel Alexandre Pereira do Nascimento 
(01800433)

Cleydson Barbosa da Silva Ramos
(01786045)

Pré-requisitos

Node.js 24.22.1 ou superior;
pnpm 9, 10 ou 11;
projeto Payload conectado pelo Figma Make;
variáveis de ambiente configuradas para o envio de e-mails.
Variáveis de ambiente
As credenciais não devem ser adicionadas ao Git. Configure-as nos segredos do Figma Make:

RESEND_API_KEY
RESEND_FROM_ADDRESS
O Figma Make fornece automaticamente as variáveis internas necessárias ao Payload.

Instalação e execução
Clone o repositório:

git clone URL_DO_REPOSITORIO
cd NOME_DO_REPOSITORIO
Instale as dependências:

pnpm install
Inicie o ambiente de desenvolvimento:

pnpm dev
A aplicação ficará disponível em http://localhost:3000.

Comandos disponíveis
pnpm dev       # ambiente de desenvolvimento
pnpm build     # build de produção
pnpm start     # executa o build de produção
pnpm format    # formatação do código
Rotas principais
Rota	Descrição
/	Portal turístico
/entrar	Login
/cadastro	Cadastro
/esqueci-minha-senha	Recuperação de acesso
/redefinir-senha	Criação de nova senha
/area-restrita	Área protegida do visitante
/admin	Administração do Payload
Organização do Git
A branch principal deve ser a main. Cada funcionalidade deve ser desenvolvida em uma branch própria:

main
├── feature/navbar
├── feature/login
├── feature/cadastro
├── feature/recuperacao-senha
└── feature/area-restrita
Exemplo de criação de uma branch:

git switch main
git pull origin main
git switch -c feature/login
Padrão de commits
Cada integrante deve criar seus próprios commits. Não altere autoria e não concentre todo o trabalho em um único integrante.

Exemplos:

feat: adiciona navegação responsiva
feat: implementa formulário de login
feat: protege acesso à área restrita
fix: corrige validação do cadastro
docs: atualiza instruções de execução
Fluxo de Pull Request
Crie a branch da funcionalidade a partir da main;
faça commits pequenos e descritivos;
envie a branch para o GitHub;
abra um Pull Request para a main;
solicite a revisão de outro integrante;
o revisor deve comentar, solicitar ajustes quando necessário e aprovar;
integre o PR somente após a aprovação;
registre no relatório da entrega o link do Pull Request integrado.
Exemplo:

git push -u origin feature/login
gh pr create --base main --head feature/login
Uma aprovação real precisa ser feita pela conta de outro integrante. Não é válido inventar revisões ou alterar a autoria dos commits.

Checklist para entrega
 URL do repositório GitHub preenchida neste README;
 nomes e usuários dos integrantes preenchidos;
 pasta node_modules ignorada;
 branch principal chamada main;
 branches de funcionalidade publicadas no GitHub;
 commits realizados pelos respectivos integrantes;
 Pull Request aberto por um integrante;
 Pull Request revisado e aprovado por outro integrante;
 Pull Request integrado à main;
 link do Pull Request anexado à entrega.
Licença
Projeto acadêmico desenvolvido para fins educacionais.
