DOCUMENTO 1: GUIA DE CRIAÇÃO DE
CONTAS
Supabase + Zapier (Passo a Passo)
PARTE 1: CRIAR CONTA SUPABASE
Passo 1: Acessar Supabase
1. Acesse: https://supabase.com
2. Clique em "Sign Up"
3. Use seu email ou GitHub
Passo 2: Criar Projeto
1. Clique em "New Project"
2. Nome: mems-diagnostico
3. Senha: Crie uma forte (salve em lugar seguro )
4. Região: South America (São Paulo) (mais rápido)
5. Clique "Create new project"
Tempo de criação: 2-3 minutos
Passo 3: Copiar Credenciais
Após criar, você verá:
• Project URL: Copie e salve
• API Key (anon): Copie e salve
• API Key (service_role): Copie e salve
Exemplo:
Plain Text
Project URL: https://xxxxxxxxxxxx.supabase.co
API Key (anon ): eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
API Key (service_role): eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
Passo 4: Ativar Extensões
1. Vá para "Extensions" (no menu esquerdo)
2. Procure por "pgvector"
3. Clique em "Install"
4. Confirme
Por que? Para busca vetorial (base de conhecimento)
PARTE 2: CRIAR CONTA ZAPIER
Passo 1: Acessar Zapier
1. Acesse: https://zapier.com
2. Clique em "Sign Up"
3. Use seu email
Passo 2: Verificar Email
1. Verifique seu email
2. Clique no link de confirmação
3. Crie sua senha
Passo 3: Criar Zap (Fluxo )
1. Clique em "Create" → "Create a Zap"
2. Você verá: "Trigger" (início) + "Action" (ação)
Não crie nada ainda. Vamos fazer no Documento 3.
Passo 4: Conectar Typeform
1. Vá para "My Apps"
2. Procure "Typeform"
3. Clique "Connect"
4. Autorize Zapier a acessar seu Typeform
Como autorizar:
• Vá para seu Typeform
• Vá para "Settings" → "Integrations"
• Gere um token de API
• Cole no Zapier
Passo 5: Conectar Supabase
1. Vá para "My Apps"
2. Procure "PostgreSQL" (Supabase usa PostgreSQL)
3. Clique "Connect"
4. Preencha:
• Host: Seu Project URL (sem https:// )
• Port: 5432
• Database: postgres
• User: postgres
• Password: A senha que você criou
Exemplo:
Plain Text
Host: xxxxxxxxxxxx.supabase.co
Port: 5432
Database: postgres
User: postgres
Password: SuaSenhaForte123!
Passo 6: Conectar OpenAI
1. Vá para "My Apps"
2. Procure "OpenAI"
3. Clique "Connect"
4. Cole sua API Key do OpenAI
PARTE 3: CONECTAR OPENAI (Se não tiver)
Se você JÁ tem API Key:
Pule para "PARTE 4"
Se você NÃO tem:
1. Acesse: https://platform.openai.com/api/keys
2. Clique "Create new secret key"
3. Copie a chave (você não consegue ver depois )
4. Salve em lugar seguro
Custo: Você paga por uso (R$ 0,15-0,30 por diagnóstico)
PARTE 4: TESTAR CONEXÕES
Testar Supabase
1. No Zapier, crie um Zap de teste
2. Escolha "PostgreSQL" como trigger
3. Teste a conexão
4. Se funcionar, aparece ✅
Testar OpenAI
1. No Zapier, escolha "OpenAI" como action
2. Teste a conexão
3. Se funcionar, aparece ✅
Testar Typeform
1. No Zapier, escolha "Typeform" como trigger
2. Teste a conexão
3. Se funcionar, aparece ✅
RESUMO: O QUE VOCÊ TEM AGORA
✅ Conta Supabase (banco de dados)
✅ Conta Zapier (orquestração)
✅ Conexão Typeform → Zapier
✅ Conexão Zapier → Supabase
✅ Conexão Zapier → OpenAI
PRÓXIMO PASSO
Vá para Documento 2: Estrutura Supabase
Lá você vai criar as tabelas e estrutura do banco.
TEMPO TOTAL DESTA PARTE
⏱️ 30 minutos
• Criar Supabase: 5 min
• Criar Zapier: 5 min
• Conectar tudo: 15 min
• Testar: 5 min
