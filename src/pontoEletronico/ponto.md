table registroponto {
  registroponto_id            integer [primary key]
  usuario_id                  integer [not null]
  pessoa_id                   integer [not null]
  registroponto_tipo          varchar [not null] // entrada ou saida
  registroponto_justificativa varchar
  registroponto_inclusao      timestamp
  registroponto_exclusao      timestamp
}

Funcoes
- Registrar ponto
- Registrar justificativa
