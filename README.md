# Liquid Mask Animated Button

Este projeto apresenta um botão com um design orgânico e complexo, utilizando **Máscaras SVG** e animações de preenchimento lateral. É um exemplo avançado de como recortar elementos HTML usando caminhos vetoriais e criar transições suaves de estado.

---

## 🚀 Destaques Técnicos

### 1. Máscara SVG Customizada (`mask-image`)
O diferencial deste botão é o uso da propriedade `mask-image` (e `-webkit-mask`). Em vez de um retângulo simples, o botão é recortado por um caminho SVG complexo injetado via Data URI. Isso permite criar formas irregulares e orgânicas que seriam impossíveis de alcançar apenas com `border-radius`.

### 2. Efeito de Preenchimento Central
O botão utiliza o pseudo-elemento `:before` para criar um efeito de carregamento ou preenchimento:
* **Estado Inicial**: O preenchimento tem `width: 0`, posicionado no centro (`left: 50%`).
* **Hover**: A largura expande para `100%` em uma transição de 1 segundo, preenchendo o botão de dentro para fora.

### 3. Glow Externo Suave
Através do pseudo-elemento `:after`, o botão projeta um brilho esbranquiçado (`#ffffffa6`) ao passar o mouse. O uso de `box-shadow` com uma transição lenta de 2 segundos confere um aspecto etéreo e moderno à interação.

### 4. Tipografia Dinâmica
O texto "PLAY NOW" alterna entre preto e branco conforme o fundo é preenchido pela animação. O espaçamento de letras (`letter-spacing: 3px`) e o peso leve (`font-weight: 100`) reforçam a estética minimalista e premium.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5**: Estrutura de botão simples.
* **CSS3 Avançado**: 
    - `mask-image`: Para o recorte da forma orgânica.
    - `pseudo-elements` (`:before` e `:after`): Para as camadas de animação e luz.
    - `transitions`: Controle preciso de tempo para preenchimento e cor.
    - `Data URI`: Para embutir o código SVG diretamente no CSS.

---

## 📂 Como Implementar

O componente depende de um arquivo CSS que suporte as propriedades de máscara:

```html```
<button class="button5">
    <span>PLAY NOW</span>
</button>

<img width="266" height="67" alt="Image" src="https://github.com/user-attachments/assets/31d0d33b-5ae7-40cd-9198-3d4567253ba9" />
