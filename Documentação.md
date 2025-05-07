# Arte Digital - Documentação

Este projeto é um site interativo que gera arte digital baseada em entradas de texto. Cada caractere, palavra ou símbolo digitado pelo usuário é interpretado para criar formas, cores e padrões únicos na tela. Abaixo está a descrição detalhada de todas as funcionalidades implementadas.

---

## Funcionalidades Gerais

1. **Entrada de Texto**:
   - O usuário pode digitar qualquer texto no campo de entrada e clicar no botão "Criar Arte" para gerar a arte correspondente.

2. **Canvas Responsivo**:
   - O site utiliza um elemento `<canvas>` que ocupa toda a tela, ajustando-se automaticamente ao tamanho da janela.

3. **Cor de Fundo Dinâmica**:
   - A cor de fundo muda dinamicamente com base no horário atual, criando uma experiência visual única a cada momento.

---

## Funcionalidades Baseadas em Caracteres

### Letras Específicas
- **W**: Desenha 21 quadrados coloridos em posições aleatórias.
- **Y**: Desenha 21 triângulos coloridos em posições aleatórias.
- **K**: Desenha 80 pontos coloridos em posições aleatórias.

### Sílabas Específicas
- **`cha`, `che`, `chi`, `cho`, `chu`**:
  - Criam manchas abstratas com degradês em tons específicos:
    - `cha`: Tons de azul.
    - `che`: Tons de marrom.
    - `chi`: Tons de amarelo.
    - `cho`: Tons de vermelho.
    - `chu`: Tons de verde.

- **`lha`, `lhe`, `lhi`, `lho`, `lhu`** e **`nha`, `nhe`, `nhi`, `nho`, `nhu`**:
  - Criam manchas abstratas com degradês em tons específicos:
    - `lha` e `nha`: Tons de roxo.
    - `lhe` e `nhe`: Tons de cinza.
    - `lhi` e `nhi`: Tons de laranja.
    - `lho` e `nho`: Tons de rosa.
    - `lhu` e `nhu`: Tons de ciano.

### Letras Acentuadas
- Letras como `á`, `é`, `í`, `ó`, `ú` desenham pequenos círculos coloridos no ponto correspondente.

### Números
- **Números juntos** (ex.: `102`):
  - Desenham a quantidade correspondente de bolinhas coloridas.
- **Números separados** (ex.: `2 amanhã 5`):
  - Somam os valores e desenham a soma correspondente de bolinhas coloridas.

---

## Funcionalidades Baseadas em Palavras

### Palavras Específicas
- **"Pablo"**:
  - Exibe a frase **"Cantando apesar das chamas."** no centro da tela, com um degradê de chamas (vermelho, laranja e amarelo).

- **"Ane"**:
  - Preenche a tela de branco e desenha um coração vermelho gigante no centro.

---

## Funcionalidades Baseadas em Símbolos

- **`!` ou `?`**:
  - Desenham duas barras verticais coloridas no fundo da tela, com cores calculadas dinamicamente com base no horário atual.

---

## Funcionalidades de Arte Abstrata

- **Traços e Curvas**:
  - Cada caractere da entrada gera traços e curvas abstratas no canvas:
    - Alterna entre linhas retas, curvas quadráticas e curvas Bézier.
    - A posição, tamanho e grossura dos traços são calculados com base no caractere.

- **Formas Aleatórias**:
  - Além dos traços, formas geométricas como círculos, quadrados e triângulos são desenhadas com cores e tamanhos aleatórios.

---

## Detalhes Técnicos

1. **Canvas**:
   - O elemento `<canvas>` é usado para desenhar todas as formas e padrões.
   - O contexto 2D (`ctx`) é utilizado para manipular os desenhos.

2. **Cálculo de Posições**:
   - As posições dos elementos são calculadas de forma determinística com base nos caracteres da entrada, garantindo que a mesma entrada sempre gere o mesmo padrão.

3. **Cores Dinâmicas**:
   - As cores são geradas dinamicamente usando valores aleatórios ou baseados no horário atual.

4. **Interatividade**:
   - O botão "Criar Arte" processa a entrada do usuário e atualiza o canvas em tempo real.

---

## Como Usar

1. Abra o site em um navegador.
2. Digite qualquer texto no campo de entrada.
3. Clique no botão "Criar Arte".
4. Observe a arte gerada no canvas.

---

## Easter Eggs

- **"Pablo"**:
  - Exibe a frase "Cantando apesar das chamas." com um degradê de chamas.
- **"Ane"**:
  - Exibe um coração vermelho gigante no centro da tela.

---

## Possíveis Melhorias Futuras

1. Adicionar mais padrões e formas baseados em caracteres ou palavras.
2. Permitir que o usuário salve a arte gerada como uma imagem.
3. Implementar animações para as formas e traços.
4. Adicionar suporte para mais símbolos e combinações de caracteres.

---

## Créditos

- Desenvolvido com criatividade e diversão para explorar arte digital interativa.