# 🐱 Cat Gallery

Mini-aplicação web que consome a API pública **The Cat API** para renderizar uma galeria responsiva de imagens aleatórias de gatos a cada carregamento de página.

---

## 🚀 Como funciona a The Cat API

A **[The Cat API](https://thecatapi.com/)** é um serviço REST gratuito que disponibiliza dados e imagens de gatos.

* **Endpoint utilizado:** `https://api.thecatapi.com/v1/images/search?limit=10`
* **Método:** `GET`
* **Parâmetro `?limit=10`:** Retorna um array com 10 objetos JSON contendo os dados e URLs das imagens.

---

## 🛠️ O que foi implementado

* **Requisição Assíncrona:** Uso de `async/await` junto com a Fetch API para buscar os dados sem travar a renderização da página.
* **Manipulação do DOM:** Criação dinâmica de tags `<img>` via `document.createElement()` e inserção no container principal com `appendChild()`.
* **Tratamento de Dados:** Conversão da resposta da API via `.json()` e iteração dos elementos com o método de array `.forEach()`.
* **Layout Responsivo:** Estruturação visual com **CSS Grid** (`repeat(auto-fit, minmax(...))`) e ajuste proporcional das fotos com `object-fit: cover`.

---

## 💻 Como executar localmente

1. Clone o repositório ou baixe os arquivos da pasta.
2. Abra o arquivo `index.html` em qualquer navegador web (ou utilize a extensão **Live Server** no VS Code).
