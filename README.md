# LUMYX

**Inteligencia que organiza sua rotina.**

LUMYX e uma plataforma inteligente de produtividade, organizacao operacional e automacao de relatorios com IA. Este MVP roda localmente no navegador e mantem as funcionalidades ja criadas: login local, dashboard, agenda, cadastro de atividades, gravacoes, resumo simulado, relatorios e exportacao em PDF.

## Como testar

1. Na pasta do projeto, rode: `npm start`
2. Abra o app em: `http://127.0.0.1:4173/`
3. Use o login de teste:
   - E-mail: `admin@lumyx.local`
   - Senha: `123456`
4. Navegue pelo menu lateral.
5. Em **Relatorios**, clique em **Gerar relatorio**.
6. Para PDF, clique em **Exportar PDF** e escolha salvar como PDF.

## Arquivos principais

- `index.html`: estrutura das telas.
- `styles.css`: identidade visual, layout e responsividade.
- `app.js`: dados locais, navegacao, gravacao, resumos e relatorios.
- `assets/lumyx-logo.png`: marca LUMYX completa.
- `assets/lumyx-mark.png`: versao compacta LM para loading e menu.
- `assets/favicon.svg`: icone do navegador.
- `server.js`: servidor local simples para teste.

## Base SaaS preparada

- `supabase/schema.sql`: estrutura inicial do banco SaaS com seguranca por organizacao.
- `supabase/fix_policies.sql`: correcao para permitir criar o primeiro workspace/perfil.
- `supabase/emergency_policies.sql`: reparo simples caso a correcao normal falhe.
- `docs/SUPABASE_SETUP.md`: guia para conectar Supabase.
- `docs/AUTH_SETUP.md`: guia para criar o primeiro usuario real.
- `docs/AI_WORKFLOW.md`: fluxo previsto para IA real.
- `docs/EXPORTS.md`: plano para PDF profissional e Word.
- `docs/DATABASE_SYNC.md`: explicacao do modo local e modo nuvem.
- `docs/OPENAI_EDGE_FUNCTION.md`: guia da funcao segura de transcricao e resumo com IA.
- `docs/ROADMAP.md`: roadmap do MVP ate SaaS.

## Proximos passos

- Conectar autenticacao real.
- Migrar dados locais para Supabase/PostgreSQL.
- Integrar IA real para transcricao, resumo e documentos.
- Exportar Word alem de PDF.
