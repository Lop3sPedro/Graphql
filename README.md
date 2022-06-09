# graphql

Problemas que o GraphQL resolve:
-Overfetching === buscar informações demais.
EX: se quiser pegar um energético o REST teria retornado uma geladeira com energético, já o GRAPHQL faz a busca expecifica deo ittem em si.

-Underfetching === buscar dados de menos.
EX: uma rota de usuarios só retorna usuários, mas é necessário ter retornar usuários e endereço, então teria q ser feita uma nova rota que iria retornar apensas os endereço.

Dificuldades do GraphQL:
-Cache (Lidar com o cache de requisições)
-Erros

```gql == ele faz uma busca mais seletiva, pegado apenas o dado necessário para a aplicação.
query {
  users {
    id
    name
    github

    addresses {
      city
      state
      country
    }
  }
}
```
