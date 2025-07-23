# Controle do Direito - Website Landing Page

## Descrição do Projeto

Website responsivo de página única (one page) desenvolvido para promover o curso de Direito Empresarial e Compliance da "Controle do Direito". O site foi criado com foco em conversão e persuasão, direcionado para advogadas recém-formadas ou com baixa remuneração.

## Características Principais

### Design e Visual
- **Paleta de cores**: Baseada no roxo (#6B46C1) do logo fornecido
- **Design moderno**: Layout limpo e profissional
- **Responsivo**: Adaptável para desktop, tablet e mobile
- **Imagens ilustrativas**: Advogados no mercado corporativo
- **Logo personalizado**: Logo criado com balança da justiça e elementos de controle
- **Banner limpo**: Banner roxo sem texto para foco no conteúdo
- **Header roxo**: Background do header na cor do banner para consistência visual

### Funcionalidades Novas
- **Tema Dark/Light**: Toggle para alternar entre temas claro e escuro
- **Persistência de tema**: Salva a preferência do usuário no localStorage
- **Transições suaves**: Animações entre mudanças de tema
- **Ícones dinâmicos**: Ícone do toggle muda conforme o tema (lua/sol)

### Seções do Site
1. **Header**: Navegação fixa com logo, menu e toggle de tema
2. **Hero**: Seção principal com proposta de valor
3. **Problema**: Identifica dores da persona Carolina
4. **Solução**: Apresenta o curso como solução
5. **Benefícios**: O que será aprendido no curso
6. **Transformação**: Antes vs Depois
7. **Preço**: Investimento e condições de pagamento
8. **Urgência**: Oferta por tempo limitado
9. **Footer**: Links e redes sociais

### Funcionalidades
- **Countdown timer**: Cria urgência na oferta
- **Scroll suave**: Navegação fluida entre seções
- **Animações**: Elementos aparecem ao rolar a página
- **WhatsApp flutuante**: Botão de contato direto
- **Vídeo YouTube**: Incorporado na seção de solução
- **Botões CTA**: Redirecionam para Hotmart
- **Cookie consent**: Conformidade com LGPD
- **Tema dark/light**: Alternância entre temas

### Técnicas de Persuasão
- **Prova social**: Depoimento da Carolina
- **Escassez**: Apenas 50 vagas disponíveis
- **Urgência**: Countdown de 24 horas
- **Garantia**: 7 dias ou dinheiro de volta
- **Parcelamento**: 12x sem juros
- **Antes/Depois**: Transformação clara
- **Benefícios específicos**: Salário de até R$ 12.000

## Estrutura de Arquivos

```
controle-direito/
├── index.html          # Página principal
├── styles.css          # Estilos CSS responsivos com tema dark
├── script.js           # JavaScript interativo com toggle de tema
├── README.md           # Documentação
└── assets/
    └── images/
        ├── new_logo.png       # Logo personalizado criado
        ├── new_banner.png     # Banner roxo sem texto
        ├── hero-lawyer.jpg    # Imagem hero
        ├── success-lawyer.jpg # Advogada de sucesso
        └── office-modern.jpg  # Escritório moderno
```

## Como Usar

### 1. Hospedagem
- Faça upload de todos os arquivos para seu servidor web
- Certifique-se de que a estrutura de pastas seja mantida
- O arquivo `index.html` deve estar na raiz

### 2. Configurações Necessárias

#### Links do Hotmart
Atualize os links nos botões de compra:
```html
<!-- Substitua por seu link real do Hotmart -->
<a href="https://hotmart.com/pt-br/marketplace/produtos/controle-do-direito">
```

#### Vídeo do YouTube
Substitua o ID do vídeo na seção de solução:
```html
<!-- Substitua dQw4w9WgXcQ pelo ID do seu vídeo -->
<iframe src="https://www.youtube.com/embed/SEU_VIDEO_ID">
```

#### WhatsApp
Configure o número do WhatsApp no script.js:
```javascript
// Linha 224 - substitua pelo número real
whatsappButton.href = 'https://wa.me/5511999999999?text=...';
```

#### Redes Sociais
Atualize os links das redes sociais no footer:
```html
<a href="https://instagram.com/SEU_PERFIL" target="_blank">
<a href="https://facebook.com/SEU_PERFIL" target="_blank">
<!-- etc... -->
```

### 3. Personalização

#### Cores
Para alterar as cores, edite as variáveis CSS no início do arquivo `styles.css`:
```css
:root {
    --primary-color: #6B46C1;    /* Cor principal */
    --secondary-color: #EC4899;   /* Cor secundária */
    --accent-color: #F59E0B;      /* Cor de destaque */
}

/* Dark Theme Variables */
[data-theme="dark"] {
    --text-dark: #F9FAFB;
    --text-light: #D1D5DB;
    --white: #1F2937;
    /* ... outras variáveis do tema dark */
}
```

#### Textos
Todos os textos podem ser editados diretamente no arquivo `index.html`.

#### Imagens
Substitua as imagens na pasta `assets/images/` mantendo os mesmos nomes.

### 4. Funcionalidade de Tema

#### Toggle de Tema
O botão de toggle está localizado no header e permite alternar entre:
- **Tema Light**: Fundo claro, texto escuro
- **Tema Dark**: Fundo escuro, texto claro

#### Persistência
A preferência do usuário é salva automaticamente no localStorage e restaurada na próxima visita.

#### Customização do Tema
Para adicionar novos elementos ao tema dark, use o seletor `[data-theme="dark"]`:
```css
[data-theme="dark"] .meu-elemento {
    background-color: #374151;
    color: #F9FAFB;
}
```

## Otimizações Implementadas

### Performance
- Imagens otimizadas
- CSS com variáveis para temas
- JavaScript eficiente com event delegation
- Lazy loading para imagens
- Preload de imagens críticas

### SEO
- Meta tags otimizadas
- Estrutura semântica HTML5
- Alt text em todas as imagens
- Schema markup (pode ser adicionado)

### Conversão
- Múltiplos CTAs estratégicos
- Prova social visível
- Garantia destacada
- Facilidade de pagamento
- Design persuasivo
- Tema dark para melhor experiência

### Acessibilidade
- Contraste adequado em ambos os temas
- Botões com títulos descritivos
- Navegação por teclado
- Transições suaves

## Compatibilidade

### Navegadores
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### Dispositivos
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (320px - 767px)

### Temas
- Tema Light (padrão)
- Tema Dark (opcional)

## Manutenção

### Atualizações Regulares
1. **Countdown**: Reinicia automaticamente a cada 24h
2. **Imagens**: Podem ser substituídas conforme necessário
3. **Preços**: Facilmente editáveis no HTML
4. **Depoimentos**: Adicione mais casos de sucesso
5. **Temas**: Facilmente customizáveis via CSS

### Monitoramento
- Use Google Analytics para acompanhar conversões
- Monitore performance com PageSpeed Insights
- Teste regularmente em diferentes dispositivos
- Verifique funcionamento do toggle de tema

## Novidades da Versão Atualizada

### ✨ Novo Logo
- Logo personalizado criado com balança da justiça
- Elementos de controle integrados ao design
- Alta resolução para todas as telas
- Formato PNG com transparência

### 🎨 Novo Banner
- Banner roxo limpo sem texto
- Foco total no conteúdo da página
- Gradiente sutil para profundidade
- Consistência visual com o header

### 🌙 Tema Dark
- Toggle no header para alternar temas
- Persistência da preferência do usuário
- Transições suaves entre temas
- Ícones dinâmicos (lua/sol)
- Cores otimizadas para ambos os temas

### 💜 Header Roxo
- Background na cor do banner
- Navegação em branco para contraste
- Botão de tema integrado ao design
- Consistência visual total

## Suporte Técnico

Para dúvidas sobre implementação ou customização:
1. Verifique este README primeiro
2. Teste as alterações em ambiente local
3. Mantenha backup dos arquivos originais
4. Use as ferramentas de desenvolvedor do navegador para debug

## Licença

Este projeto foi desenvolvido especificamente para "Controle do Direito" e não deve ser redistribuído sem autorização.

---

**Desenvolvido com foco em conversão, experiência do usuário e acessibilidade.**

