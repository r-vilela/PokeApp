# PokeApp

Este é um aplicativo Android simples desenvolvido em Java usando Android Studio. Ele consome a PokéAPI para listar Pokémon com base em seu tipo (como "fire", "water", "grass", etc.).

## Tecnologias e Bibliotecas

- Java
- Android Studio
- Retrofit
- Gson
- RecyclerView
- Intent
- SharedPreferences

## API - PokeApi

Essa API é vital para o app, utilizada em todas as funcionalidades, ao fazer a pesquisa aos pokemon pelos tipos, para buscar os dados do pokemon, para exibir a imagem, entre outros usos.

## ⚙️ Como funciona

Busca de Pokémon por tipo

O usuário digita o tipo do Pokémon no campo de texto (por exemplo: fire, water).

Ao clicar no botão de busca, uma requisição é feita à PokéAPI.

Os Pokémon retornados são exibidos em um RecyclerView.

Detalhes de um Pokémon

Ao clicar em um Pokémon da lista, uma nova Activity é aberta exibindo:

- Nome
- Foto
- ID
- Altura
- Peso
- Botão com link para mais informações via PokéAPI (abre no navegador)
- Ícone de coração indicando se ele está ou não nos favoritos:
 - Coração vermelho: Pokémon já está nos favoritos
 - Coração preto: Pokémon ainda não está nos favoritos

Esses dados são passados entre as telas usando Intent.

## Favoritar um Pokémon

Ao clicar no coração, o Pokémon é adicionado aos favoritos.

Os dados do Pokémon são convertidos em JSON usando Gson.

Esses dados são armazenados em um arquivo local chamado favorites_pokemons.xml.

## Lista de Favoritos

Na tela principal, há um botão em formato de coração.

Ao clicar nele, o app:

- Lê o arquivo favorites_pokemons.xml
- Percorre todos os Pokémon favoritados
- Exibe essa lista em um RecyclerView

## ▶️ Como rodar

Clone o repositório:
```
git clone https://github.com/seu-usuario/pokedex-por-tipo.git
```

Abra o projeto no Android Studio.

Conecte um dispositivo físico ou inicie um emulador.

Execute o app.
