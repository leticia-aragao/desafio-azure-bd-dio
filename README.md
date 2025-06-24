# Desafio Azure Banco de Dados - DIO

## 📌 Descrição
Este repositório tem como objetivo documentar a experiência adquirida durante o laboratório da DIO sobre a criação de uma instância de banco de dados SQL no Azure.

## 🛠️ Etapas
1. Entre no portal da Azure, selecione Todos os serviços e, em seguida, digite SQL do Azure na caixa de pesquisa. Aperte em "Criar".

2. Na aba "Básico", preencha as informaões obrigatórias, que são os requisitos mínimos para provisionar uma Instância Gerenciada de SQL.
    - Assinatura: selecionar a assinatura para gerenciar os custos e os recursos implantados.
    - Grupo de recursos: organizar e gerenciar todos os seus recursos.
    - Nome do banco de dados: definir um nome
    - Servidor: criar um novo servidor ou utilizar um existente
    - Pertence a um pool de instâncias: para que a instância seja criada dentro de um pool de instâncias.
    - Computação + armazenamento: escolher uma camada de Serviço SQL e um nível de desempenho.

3. Na aba "Rede", configure o acesso à rede e a conectividade do servidor (são informações opcionais).
    - Regras de Firewall: define quem pode acessar o servidor SQL com base em endereços IP autorizados.
    - Pontos de extremidade privados: permite conexões seguras via IPs privados dentro de uma Rede Virtual do Azure.
    - Política de conexão: controla como os clientes se conectam ao banco de dados.
    - Conexões criptografadas: define o protocolo mínimo de segurança (TLS) usado para proteger os dados em trânsito.

4. Na aba "Segurança", proteger os dados usando o Microsoft Defender para SQL.
    - Microsoft Defender para SQL: fornece segurança avançada com detecção de ameaças e avaliação de vulnerabilidades.
    - Razão: garante a integridade dos dados por meio de verificação criptográfica contra alterações ou violações.
    - Identidade do servidor: controla o acesso a recursos com identidades gerenciadas.
    - Gerenciamento transparente de chaves de criptografia de dados: criptografa dados em repouso automaticamente.
    - Always Encrypted: protege dados sensíveis até mesmo de administradores.

5. Na aba "Configurações adicionais", são informações opcionais, se não forem preenchidas, o portal aplicará as configurações padrão.
    - Fonte de dados: define como o banco será criado — em branco, com backup ou com dados de exemplo.
    - Ordenação do banco de dados: define regras de comparação e ordenação de texto, que não podem ser alteradas depois.

6. Na aba "Rótulos", é possivel criar marcas, que são pares de nome/valor que permitem classificar recursos.
    - Útil em empresas com muitos recursos.
    - Opcional, mas boa prática incluir no projeto.

7. Na aba “Revisar + Criar”, confirma se tudo está certo antes de criar a instância de banco de dados.
   - O Azure vai validar as configurações.
   - Se estiver tudo OK, clique em “Criar”.
