# Documentação do Site BellaDonna

## 📑 Índice
1. [Visão Geral](#visão-geral)
2. [Estrutura do Projeto](#estrutura-do-projeto)
3. [Componentes](#componentes)
4. [Estilização](#estilização)
5. [Responsividade](#responsividade)
6. [JavaScript](#javascript)

## 🎯 Visão Geral
O BellaDonna é uma landing page moderna para um salão de beleza, desenvolvida com HTML5, CSS3 e JavaScript. O site apresenta um design elegante e responsivo, com foco na experiência do usuário e na apresentação dos serviços oferecidos.

## 📁 Estrutura do Projeto
```
exec-senai_landing-page/
├── src/
│   ├── index.html
│   ├── assets/
│   │   ├── pexels-alexander-mass-galeria.jpg
│   │   ├── pexels-cottonbro-contato.jpg
│   │   ├── pexels-heru-dharma.jpg
│   │   └── pexels-valeriya-galeria.jpg
│   └── css/
│       └── style.css
```

## 🧩 Componentes

### 1. Header
- Menu de navegação responsivo
- Logo do salão
- Menu hamburguer para dispositivos móveis
- Links para as seções principais
```html
<header>
    <h1>LogoSalaoBeleza</h1>
    <nav class="menu">...</nav>
</header>
```

### 2. Hero Section
- Imagem em tela cheia com overlay
- Texto de chamada principal
- Botão CTA (Call to Action)
```html
<section class="hero">
    <img src="assets/pexels-heru-dharma.jpg" alt="salao de beleza">
    <div class="hero-content">...</div>
</section>
```

### 3. Seção Sobre
- Apresentação do salão
- Cards com destaques
- Ícones informativos
- Layout em grid responsivo

### 4. Seção Serviços
- Cards de serviços
- Ícones ilustrativos
- Lista de características
- Botões de agendamento

### 5. Galeria
- Grid de imagens
- Efeitos de hover
- Overlay com descrição
- Layout responsivo

### 6. Footer
- Informações de contato
- Horário de funcionamento
- Links para redes sociais
- Copyright

## 🎨 Estilização

### Variáveis CSS
```css
:root {
    --primary-color: #c2185b;
    --primary-light: #f8b6d2;
    --text-color: #333;
    --header-height: 80px;
}
```

### Destaques de Estilo
1. **Gradientes**
   - Header: `linear-gradient(90deg, var(--primary-light) 0%, #fff 100%)`
   - Footer: `linear-gradient(135deg, var(--primary-color) 0%, #8e0d3c 100%)`

2. **Efeitos de Hover**
   - Transformações suaves
   - Mudanças de cor
   - Overlays
   - Sombras dinâmicas

3. **Cards**
   - Sombras sutis
   - Bordas arredondadas
   - Transições suaves
   - Estados hover interativos

## 📱 Responsividade

### Breakpoints
```css
/* Desktop */
@media (min-width: 1200px) {
    /* Estilos para telas grandes */
}

/* Tablet */
@media (max-width: 900px) {
    /* Ajustes para tablets */
}

/* Mobile */
@media (max-width: 700px) {
    /* Layout mobile */
}
```

### Características Responsivas
- Menu hamburguer em telas pequenas
- Grid adaptável
- Fontes responsivas com `clamp()`
- Imagens otimizadas
- Layout flexível

## 🔧 JavaScript

### Menu Responsivo
```javascript
const menuToggle = document.getElementById('menu-toggle');
const menuList = document.getElementById('menu-list');

menuToggle.addEventListener('click', () => {
    menuList.classList.toggle('active');
});

// Acessibilidade
menuToggle.addEventListener('keypress', (e) => {
    if (e.key === 'Enter' || e.key === ' ') {
        menuList.classList.toggle('active');
    }
});
```

## 🎯 Recursos e Bibliotecas
- **Font Awesome**: Para ícones
- **Google Fonts**: Para tipografia
- **Normalize.css**: Para consistência entre navegadores

## ⚡ Performance e Otimizações
1. Imagens otimizadas
2. CSS minificado
3. Carregamento eficiente de fontes
4. Código JavaScript modular

## 🌟 Boas Práticas Implementadas
1. HTML semântico
2. CSS organizado e comentado
3. Código responsivo
4. Acessibilidade básica
5. Performance otimizada
