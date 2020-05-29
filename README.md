# Clients

- Web:
  - Administração.
  - Vendedor (Offline & Mobile first).
  - Cliente.

# O que o sistema precisa fazer?

<!-- - Integrar com SIAGRI:
  - Extrair dados já existentes de cada cliente:
    - Base de cadastro.
    - Histórico de vendas:
      - Safra.
      - Ano. -->

- Dados dos Cliente:
  - Dados pessoais:
    - Nome.
    - E-mail.
    - Telefone de contato.
    - Data de nascimento.
  - Vendas:
    - Sim.
    - Não.
  - Efetivado:
    - Sim.
    - Não.
  - Propriedades (Possível cadastrar mais de uma fazenda):
    - Micro região.
    - Endereço.
    - Localização.
    - Talhão (Possível cadastrar mais de um):
      - Nome.
      - Tamanho da área.
    - Gerente da fazenda:
      - Nome.
      - E-mail
      - Telefone de contato.
      - Data de nascimento.
    - Consultor:
      - Nome.
      - E-mail
      - Telefone de contato.
      - Data de nascimento.
- Dados de vendedores:
  - Nome.
  - E-mail.
  - Telefone de contato.
  - Status:
    - Ativo.
    - Inativo.
- Fazer pré-cadastro de cliente:
  - Necessita da permissão do ADMIN para efetivar.
- Registro de visita.
- Histórico de visitas por Vendedor, Cliente, Safra, Fazenda e Talhão.
- Relatório de fechamento de Safra:
  - Conter todos os relatórios gerados para o cliente.
  - Horas e quantidade de visitas técnicas.

## RN

- Vendedor é único para cada Cliente. (Responsável)

# O que o usuário irá fazer?

## ADMIN

- Login.
- Recuperação de senha.
- Atualizar dados:
  - E-mail.
  - Senha.
- Cadastrar / Visualizar / Atualizar / Deletar:
  - Clientes.
  - Vendedores.
- Visualizar solicitação de cadastros (Pré-cadastros):
  - Efetivar/Recusar cadastro.
- CRUD de Planejamento das visitas para cada cliente:
  - Safra.
  - Vendedor.
  - Cliente -> Fazenda -> Talhão:
    - Data de plantio.
    - Cultura:
      - Soja.
      - Milho.
    - Calendário:
      - Datas de visitas obrigatórias.
      - Tipos de visitas designadas (Depende do tipo da cultura):
        - S1;
        - S2;
        - ...
        - M1;
        - M2;
        - ...
      - Descrição.
- Acompanhar todos os planejamentos de visitas de clientes e vendedores.
- Visualizar / Gerar:
  - Histórico de visitas de cada vendedor e cliente.
  - Filtros aplicáveis:
    - Safra.
    - Vendedor.
    - Cliente.
    - Fazenda.
    - Cultura:
      - Soja.
      - Milho.

## Vendedor

- Login.
- Recuperação de senha.
- Atualizar dados:
  - Telefone.
  - E-mail.
  - Senha.
- Carteira de clientes:
  - Visualizar todos clientes.
  - Fazer pré-cadastro.
  - Visualizar Planejamento de cada cliente.
- Visitas agendadas (Calendário):
  - Dia.
  - Cliente.
  - Fazenda:
    - Micro região.
    - Talhão.
  - Visualizar:
    - Visitas para o dia seguinte.
    - Todas as visitas futuras.
- Visita:
  - Selecionar Cliente -> Fazenda -> Talhão.
  - Informar data de plantio para cada talhão.
  - Escolher qual tipo de visita:
    - S1;
    - S2;
    - ...
    - M1;
    - M2;
    - ...
  - Tirar fotos das plantas e descrever (opcional) cada uma.
  - Conter localização da foto (opcional).
  - Fazer descrição de cada visita.
  - Gerar relatório da visita para o Cliente.
  - Fazer checking e checkout para as visitas técnicas.

## Cliente

- Login.
- Alterar cadastro:
  - Telefone.
  - E-mail.
  - Senha.
- Visualizar:
  - Fazendas cadastradas.
  - Vendedor responsável:
    - Nome.
    - E-mail.
    - Telefone.
  - Histório de visitas.
  - Relatórios de visitas.

# Referências:

- QION
- Clover CRM
- TBDC consultoria e timeline

## Integração com SIAGRI

6436201500 (Suporte Jataí)

Necessário abrir um chamado com suporte técnico especificando quais informações irá utilizar:

- Base de clientes.
- Produtos.

Case seja necessário vender um produto para um cliente diretamente pelo app e constar no SIAGRI, também é necessário informar essa funcionalidade.
