# Cronômetro DFTE_UFRN

Este repositório contém um cronômetro digital de uso laboratorial, desenvolvido para o Departamento de Física Teórica e Experimental da UFRN. O projeto utiliza Arduino/ESP32, com o código principal em arquivo `.ino`, e peças impressas em 3D para montagem do gabinete.

---

## Principais características do arquivo .ino (Arduino/ESP32)

- **Linguagem/Compatibilidade**: Código em C++ próprio para Arduino, ESP32 ou similares.
- **Estrutura típica**:
    - Definição de pinos para botões, display, LEDs, etc.
    - Inicialização de periféricos no `setup()`.
    - Loop principal para leitura de botões e atualização do display.
    - Funções auxiliares para debounce, controle de estado, e lógica de contagem.
- **Operações suportadas:**
    - Iniciar, pausar e resetar o cronômetro.
    - Exibição precisa do tempo (até milissegundos, se desejado).
    - Indicação visual (LEDs, display) e sonora (se houver buzzer).
- **Flexível e comentado:** Fácil adaptação do código e documentação com comentários para aprendizado ou modificações.

---

## Lista de Componentes Eletrônicos

| Qtde | Descrição                  | Designador          | Fabricante/Supplier    | Parte/Fabricante     | Código LCSC     |
|------|----------------------------|---------------------|------------------------|----------------------|-----------------|
| 1    | ESP32 DEVKITV1             | -                   | -                      | ESP32-DEVKITV1       | -               |
| 1    | Suporte p/ Bateria 18650   | U12                 | -                      | BAT_BOX              | C9900015078     |
| 1    | Regulador de Tensão        | U4                  | -                      | 134N3P COPY          | -               |
| 9    | Conector Banana (painel)   | U1-U3, U6-U11       | -                      | Any Banana Jack      | -               |
| 1    | Conector 2P KH-PH-2P-Z     | CN1                 | kinghelm               | KH-PH-2P-Z           | C2898945        |
| 3    | Capacitor 0805             | C1, C2, C3          | -                      | -                    | -               |
| 3    | LED RGB WS2812B-5050       | LED1-LED3           | -                      | WS2812B-5050RGB      | C2838584        |
| 6    | Push button 6x6x7mm        | KEY1-KEY6           | ReliaPro               | 6*6*7                | C69055          |
| 1    | Módulo LCD 1.8"            | LCD1                | Waveshare              | 1.8INCH LCD MODULE   | C359940         |
| 4    | MOSFET LBSS138LT1G-VB      | Q1-Q4               | VBsemi                 | LBSS138LT1G-VB       | C7429063        |
| 9    | Resistor 0805 10k          | R1, R2-R9           | -                      | 0805_10k             | C9900012714     |
| 1    | Chave CN-KCD1-101-2P       | SW1                 | -                      | CN-KCD1-101-2P       | C9900002516     |

> Consulte a BOM completa para detalhes adicionais: `BOM_PhotoGate_Controlador_2026-05-15.csv`.

---

## Lista de Peças para Impressão 3D

1. **Gabinete Principal:** Estrutura para acomodar o ESP32, LCD, botões e conectores.
2. **Frontal do Gabinete:** Painel com janelas/furos para display, LEDs e botões.
3. **Tampa Traseira:** Fecho para o gabinete, com furos para fixação se necessário.
4. **Suporte para a bateria 18650:** (opcional, conforme design).
5. **Botões personalizados para painel:** (opcional, melhor ergonomia/estética).
6. **Bases ou pés para apoio:** (opcional, estabilidade em bancada).

> Os arquivos STL necessários para impressão estarão na pasta `/impressao_3d` deste repositório.

---

## Montagem e Funcionamento

1. **Imprima as peças 3D** conforme necessário.
2. **Monte o ESP32, display e botões** no gabinete impresso.
3. **Realize a ligação dos botões, display e LEDs** de acordo com o que está especificado no `.ino` e na tabela de componentes.
4. **Alimente o circuito** via USB ou bateria (18650, conforme montagem).
5. **Carregue e rode o código** na ESP32 usando a IDE Arduino.
6. **Operação**: utilize os botões para iniciar, pausar ou resetar. O tempo será mostrado no LCD, e LEDs poderão sinalizar o status.

---

## Recomendações e Observações

- Confirme o mapeamento dos pinos entre hardware e código.
- Use resistores de pull-down nos botões para evitar disparos falsos.
- Realize testes antes de fechar o gabinete definitivamente.
- Adapte o código caso utilize um display/módulo diferente.
- Instale quaisquer bibliotecas necessárias na IDE Arduino antes do upload.

---

## Licença

[uso livre]

---

**Dúvidas, sugestões ou problemas?**  
Abra uma issue neste repositório.
