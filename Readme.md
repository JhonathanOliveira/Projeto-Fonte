# Projeto de uma Fonte - SSC0180 Eletrônica para Computação - USP São Carlos
## Objetivo
Projetar uma fonte que receba uma tensão RMS de 127V de corrente alternada com 60Hz e tenha como saída uma corrente continua constante de tensão ajustável entre 3V a 12V com capacidade de 100mA.
### Transformador
Adequa o nível de tensão proveniente da rede para o nível de tensão desejada.
![image](https://user-images.githubusercontent.com/85267964/127164862-07adb976-c8f4-4557-b152-b2d6b548307e.png)
### Retificação
Transforma a corrente que antes era alternada em uma corrente continua pulsante através da "transformação" dos semiciclos negativos em positivos usando uma ponte de Diodos.

![image](https://user-images.githubusercontent.com/85267964/127166412-4c9c36d0-ad5e-412c-b154-9f382b30c371.png)
### Filtragem
Atenua os "vales" que podem ser vistos no gráfico, para isso usamos um capacitor. O Ripple é o novo valor da oscilação da tensão e é medido em porcentagem da oscilação original.

![image](https://user-images.githubusercontent.com/85267964/127168437-bdf94fe7-8d51-4534-be1c-ea9c8bd4ba4e.png)
### Regulação
Essa é a ultima etapa e consiste em tornar a corrente continua em constante, para isso vamos "cortar" a parte abaixo do pico mínimo do ripple usando um diodo zener, dessa forma não teremos mais oscilações. Nesta etapa também vamos tornar a tensão ajustável usando um potenciômetro.

![image](https://user-images.githubusercontent.com/85267964/127177226-f81f4f52-25b7-4938-bf6a-94d0d7769c33.png)
## Componentes e Preços
|Quant |Componente   |Especificações| Preço     |
|  :-: |     :-:     |     :-:      |    :-:    |
|1x    |[Transformador](https://produto.mercadolivre.com.br/MLB-1590579363-transformador-entrada-110220v-saida-17v-08a-uso-geral-_JM?matt_tool=68186480&matt_word=&matt_source=google&matt_campaign_id=12271057348&matt_ad_group_id=117812253976&matt_match_type=&matt_network=g&matt_device=c&matt_creative=496856058221&matt_keyword=&matt_ad_position=&matt_ad_type=pla&matt_merchant_id=263976801&matt_product_id=MLB1590579363&matt_product_partition_id=310938601101&matt_target_id=pla-310938601101&gclid=Cj0KCQjw9O6HBhCrARIsADx5qCREHJpLEsr8eBNputJEzBJEYFnZsiGpf34z5qbYUBKQijr2rzcTeGgaAiE9EALw_wcB)|    17V       | R$18,91|
|4x    |[Diodo](https://www.baudaeletronica.com.br/diodo-1n4007.html)        |     1N4007   |  R$0,40|
|1x|[Resistor](https://www.baudaeletronica.com.br/resistor-1k-5-1-4w.html?gclid=Cj0KCQjw9O6HBhCrARIsADx5qCRMlNaP_h1QmebZCefj1KAM79iml9dh2ZtkulPFpoBmj30TD4UAbPMaAuWsEALw_wcB)|1k|R$0,06|
|1x|[Resistor](https://www.baudaeletronica.com.br/resistor-2k-5-1-4w.html?gclid=Cj0KCQjw9O6HBhCrARIsADx5qCTXI_57t8omr_wWqVsbYg5ANadbM-3vJB5mD54eyXh_OoTI7aAWtaMaAtXAEALw_wcB)|2k|R$0,06|
|1x|[Capacitor](https://www.baudaeletronica.com.br/capacitor-eletrolitico-1000uf-16v.html)|740uF|R$0,51|
|1x|[Potenciômetro](https://www.baudaeletronica.com.br/potenciometro-linear-de-5k-5000.html)|5k|R$2,21|
|1x|[Transistor](https://www.baudaeletronica.com.br/transistor-npn-bc548.html)|NPN|R$0,19|
|1x    |  [Diodo Zener](https://www.baudaeletronica.com.br/diodo-zener-1n4743-13v-1w.html)|  13V  |R$0,21     |
| **Total**   | |             |**R$22,55**|
