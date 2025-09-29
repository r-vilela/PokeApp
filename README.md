# PokeApp

Este é um aplicativo Android simples desenvolvido em Java usando Android Studio. Ele consome a PokéAPI
 para listar Pokémon com base em seu tipo (como "fire", "water", "grass", etc.).

## Tecnologias e Bibliotecas

 - Java

 - Android Studio

 - Retrofit

 - GSON

 - RecyclerView

 - Intent

# Como funciona

O usuário digita o tipo do Pokémon no campo de texto (por exemplo: fire).

Ao clicar no botão de busca, uma requisição é feita à PokéAPI.

Os Pokémon retornados são exibidos em um RecyclerView.

Ao selecionar um Pokémon, é aberta uma nova Activity com:

 - Nome do Pokémon.

 - Botão com um Link para mais informações via API (abrindo no navegador).

## Como rodar

Clone o repositório:

git clone https://github.com/seu-usuario/pokedex-por-tipo.git


Abra no Android Studio.

Execute em um emulador ou dispositivo físico.
