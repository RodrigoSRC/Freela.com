# Buy.com

<!-- 
Table users {
  id integer [primary key]
  nome varchar
  email varchar
  password varchar
  purchases array
  created_at timestamp
}


Table products {
  id integer [primary key]
  name varchar
  category categories
  value int
  details varchar
  stock varchar
  created_at timestamp

  user_id int
}

Table images {
  id integer [primary key]
  url varchar

  product_id int
}

Table address_information {
  id integer [primary key]
  street varchar
  state states
  cep varchar
  city varchar
  number varchar
  complement varchar

  user_id int
}

Table personal_information {
  id integer [primary key]
  cpf varchar
  phone varchar
  bith_date date

  user_id int
}

Table favorites {
  id integer [primary key]

  user_id int
  product_id int
}

Table reviews_products {
  id integer [primary key]
  description varchar
  created_at timestamp

  user_id int
  product_id int

}

Table reviews_users {
  id integer [primary key]
  description varchar
  created_at timestamp
  review reviews

  author_id int
  analyzed_id int

}

Enum reviews {
  "1"
  "2"
  "3"
  "4"
  "5"
}

Enum states {
  AC
  AL
  AP
  AM
  BA
  CE
  DF
  ES
  GO
  MT
  MS
  MG
  PA
  PB
  PR
  PE
  PI
  RJ
  RN
  RS
  RR
  RO
  SC
  SP
  SE
  TO 
}

Enum categories {
  Imoveis
  Autos_e_pecas
  Casa_Decoracao_e_Utensilios
  Celulares_e_Telefonia
  Informatica
  Games
  TVs_e_video
  Audio
  Cameras_e_Drones
  Musicas_e_Hoobies
  Esportes_e_Lazer
  Artigos_Infantis
  Comercio_e_Escritorio
  Servicos
  Vagas_de_Emprego
  Eletro
  Materiais_de_Construcao
  Moveis
}



Ref: products.user_id > users.id // many-to-one

Ref: products.id < images.product_id

Ref: users.id < reviews_products.user_id

Ref: products.id < reviews_products.product_id

Ref: users.id - address_information.user_id

Ref: users.id - personal_information.user_id

Ref: users.id - favorites.user_id

Ref: products.id - favorites.product_id

Ref: users.id < reviews_users.author_id

Ref: users.id < reviews_users.analyzed_id



 -->