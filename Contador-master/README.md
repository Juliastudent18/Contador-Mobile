NOME: JULIA SOUZA COSTA

# Contador

Aplicativo Android de tela única desenvolvido em **Kotlin com Jetpack Compose**, com o objetivo de demonstrar o funcionamento de estados e recomposição no Compose.

## 📱 Sobre o projeto

O aplicativo apresenta um contador que começa com o valor `0` e possui dois botões: **Incrementar** e **Decrementar**. Ao tocar nos botões, o valor é atualizado imediatamente na tela.

O estado do contador é armazenado utilizando `remember { mutableStateOf(0) }`. Quando o valor do estado é alterado, o **Jetpack Compose detecta a mudança e realiza a recomposição** dos componentes que dependem desse estado. Dessa forma, não é necessário atualizar manualmente o texto exibido na tela.

A tela foi construída utilizando componentes do **Material 3**, `Scaffold`, `TopAppBar` e um `Composable` separado para a tela do contador.

## 👤 Autor

**Nome:** Seu Nome

## 🛠️ Tecnologias utilizadas

* Kotlin
* Android
* Jetpack Compose
* Material 3
* Android Studio

## ⚙️ Funcionalidades

* Exibição do valor atual do contador
* Contador iniciado em `0`
* Botão para incrementar o contador em `+1`
* Botão para decrementar o contador em `-1`
* Atualização imediata do valor na tela
* Interface construída com Jetpack Compose
* `Scaffold` com `TopAppBar`
* Preview da tela com `@Preview`

## 🧠 Funcionamento do estado

O contador utiliza `remember { mutableStateOf(0) }` para armazenar seu estado durante a composição.

Quando o usuário toca no botão de incrementar ou decrementar, o valor do estado é alterado.

O Compose observa essa alteração e identifica quais partes da interface dependem desse estado.

Em seguida, esses componentes são recompostos automaticamente, fazendo com que o novo valor do contador seja exibido na tela sem a necessidade de atualizar o texto manualmente.

## ⭐ Desafios opcionais

### Implementados

* [ ] **D1** — Impedir que o contador fique negativo.
* [ ] **D2** — Adicionar botão "Zerar".
* [ ] **D3** — Preservar o valor durante a rotação da tela com `rememberSaveable`.
* [ ] **D4** — Alterar a cor do número conforme o valor.
* [ ] **D5** — Utilizar `ViewModel` para controlar o estado.

> Marque com `x` os desafios que você realmente implementou.

Exemplo:

```text
- [x] D1 — Impedir que o contador fique negativo.
- [x] D3 — Preservar o valor durante a rotação da tela.
- [ ] D2 — Adicionar botão "Zerar".
- [ ] D4 — Alterar a cor do número conforme o valor.
- [ ] D5 — Utilizar ViewModel.
```

## 📸 Captura de tela

Adicione abaixo uma captura de tela do aplicativo em execução:

![Aplicativo Contador](screenshot.png)

## 📂 Estrutura

A tela principal do contador é organizada em um `Composable` próprio, separado da `MainActivity`.

```text
app/
└── src/
    └── main/
        └── java/
            └── .../
                ├── MainActivity.kt
                └── ContadorScreen.kt
```

## ▶️ Como executar

1. Clone este repositório.
2. Abra o projeto no **Android Studio**.
3. Aguarde a sincronização do Gradle.
4. Execute o aplicativo em um emulador ou dispositivo Android.
5. Utilize os botões para incrementar e decrementar o contador.

## 📚 Objetivo da atividade

Esta atividade tem como objetivo compreender o funcionamento do **estado e da recomposição no Jetpack Compose**, mostrando como alterações em um estado observado pelo Compose provocam automaticamente a atualização da interface.
