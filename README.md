# Contador

Nome: Julia Souza Costa

Aplicativo Android de tela única desenvolvido em **Kotlin com Jetpack Compose**, com o objetivo de demonstrar o funcionamento de estados e recomposição no Compose.

## 📱 Sobre o projeto

O aplicativo apresenta um contador que começa com o valor `0` e possui dois botões: **Incrementar** e **Decrementar**. Ao tocar nos botões, o valor é atualizado imediatamente na tela.

O estado do contador é armazenado utilizando `remember { mutableStateOf(0) }`. Quando o valor do estado é alterado, o **Jetpack Compose detecta a mudança e realiza a recomposição** dos componentes que dependem desse estado. Dessa forma, não é necessário atualizar manualmente o texto exibido na tela.

A tela foi construída utilizando componentes do **Material 3**, `Scaffold`, `TopAppBar` e um `Composable` próprio para a tela do contador.

## 🛠️ Tecnologias utilizadas

- Kotlin
- Android
- Jetpack Compose
- Material 3
- Android Studio

## ⚙️ Funcionalidades

- Exibição do valor atual do contador
- Contador iniciado em `0`
- Botão para incrementar o contador em `+1`
- Botão para decrementar o contador em `-1`
- Atualização imediata do valor na tela
- Interface construída com Jetpack Compose
- `Scaffold` com `TopAppBar`
- Preview da tela com `@Preview`

## 🧠 Funcionamento do estado

O contador utiliza `remember { mutableStateOf(0) }` para armazenar seu estado durante a composição.

Quando o usuário toca no botão de incrementar ou decrementar, o valor do estado é alterado.

O Compose observa essa alteração e identifica quais partes da interface dependem desse estado.

Em seguida, esses componentes são recompostos automaticamente, fazendo com que o novo valor do contador seja exibido na tela sem a necessidade de atualizar o texto manualmente.

## ⭐ Desafios opcionais

### Implementados

Marque abaixo apenas os desafios que foram realmente implementados no aplicativo:

- [ ] **D1** — Impedir que o contador fique negativo.
- [ ] **D2** — Adicionar um botão "Zerar" com estilo visual secundário.
- [ ] **D3** — Preservar o valor do contador durante a rotação da tela com `rememberSaveable`.
- [ ] **D4** — Alterar a cor do número conforme o valor.
- [ ] **D5** — Extrair o estado para uma `ViewModel` e consumi-lo na tela.

## 📸 Captura de tela

Abaixo está uma captura de tela do aplicativo em execução:

![Aplicativo Contador](screenshot.png)

## 📂 Estrutura do projeto

A tela principal do contador é organizada em um `Composable` próprio, separado da `MainActivity`.

```text
app/
└── src/
    └── main/
        └── java/
            └── .../
                ├── MainActivity.kt
                └── ContadorScreen.kt
