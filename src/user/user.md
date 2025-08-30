user ( login )
  usuario_id       integer [primary key]
  usuario_codigo   varchar [not null]
  usuario_senha    varchar [not null] // hash
  pessoa_id        integer
  usuario_ativo    status
  loja_id          integer
  usuario_inclusao timestamp
  usuario_exclusao timestamp
Funcoes
- criar usuario
- Alterar usuario
- Deletar ( inativar )
- Listar usuarios 