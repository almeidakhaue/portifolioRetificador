# Descrição do Circuito de Fonte de Alimentação

Este circuito converte a tensão alternada (AC) para uma tensão contínua regulada (DC), com filtragem e proteção. Ele é adequado para alimentar circuitos eletrônicos e sistemas embarcados.

## Componentes Principais e suas Funções

- **J2 - Conector de Entrada**  
  Permite a conexão da fonte de corrente alternada (AC) ao circuito.

- **BR1 - Ponte Retificadora**  
  Converte a corrente alternada em corrente contínua pulsante. Contém quatro diodos internos que direcionam a corrente de forma adequada.  
  - O terminal **“+”** fornece a saída positiva e o terminal **“-”** fornece a saída negativa.

- **C1, C2, C3 - Capacitores**  
  - **C1** (provavelmente cerâmico): Contribui para a estabilidade do sinal.  
  - **C2** (eletrolítico): Realiza a filtragem principal da tensão retificada, suavizando as ondulações.  
  - **C3** (provavelmente cerâmico): Melhora a resposta em altas frequências.

- **U1 - Regulador de Tensão**  
  Possivelmente um **LM7812** ou **LM7805** (dependendo da tensão de saída desejada).  
  Este componente regula a tensão de saída DC para um valor fixo.

- **R1 - Resistor**  
  Serve como limitador de corrente ou para fornecer carga a um LED indicador.

- **D1 - Diodo de Proteção**  
  Pode ser um **LED** ou um **diodo Zener**:  
  - Se for um LED, indica o funcionamento do circuito.  
  - Se for um diodo Zener, protege contra sobretensões.

- **L1 - Indutor ou Fusível (opcional)**  
  Ajuda na filtragem ou serve como proteção contra sobrecorrentes.

---

## Funcionamento do Circuito

1. **Entrada AC**  
   A tensão alternada é aplicada no conector **J2**, podendo ser proveniente de um transformador.

2. **Retificação**  
   A **ponte retificadora BR1** converte a tensão AC em uma corrente pulsante unidirecional (DC pulsante).

3. **Filtragem Inicial**  
   O capacitor **C2** suaviza a tensão retificada, reduzindo as oscilações e melhorando a forma da onda DC.

4. **Regulação da Tensão**  
   O regulador de tensão **U1** ajusta a saída para um valor fixo, como 5V ou 12V, conforme o modelo utilizado.

5. **Filtragem Final**  
   O capacitor **C3** remove ruídos de alta frequência, garantindo uma tensão mais estável.

6. **Indicação de Funcionamento**  
   Caso haja um **LED (D1)**, ele se acende, indicando que o circuito está funcionando corretamente.

---

## Aplicações

- Fontes de alimentação DC para circuitos eletrônicos.
- Conversão de tensão AC (proveniente de um transformador) para uma tensão DC regulada.
- Fontes de alimentação para microcontroladores e sistemas embarcados de pequeno porte.

---

## Contribuições

Sinta-se à vontade para contribuir com melhorias ou ajustes no código e no projeto. Abra um **Pull Request** para sugestões!

---

Se precisar de mais detalhes sobre algum componente específico, fique à vontade para perguntar! 🚀
