# Projeto Colorímetro
Projeto de construção e montagem de um colorímetro utilizando um led RGB, um smartphone, uma placa arduino e um código em python.
As peças para o trilho foram desenhadas e os desenhos em formato stl estão disponíveis para a reprodução. A montagem do trilho precisa ser complementada com 
hastes de aço de 1/4 de polegada e porcas compatíveis. O projeto utiliza um LED RGB alto brilho anodo comum tipo cápsula de 5 mm. Resistores precisam ser ligados
aos contatos do LED da sequinte forma: Contato do LED vermelho - 150 Ôhms, Contato do LED verde- 120 Ôhms e Contato do LED azul - 150 Ôhms. Eventualmente utilizando resistores de resistência um pouco menor poderá funcionar com tensão ainda anterior ao limiar dos LEDs. No trabalho de referência, foi utilizada uma cubeta de vidro comum, adquirida por 35 reais de 10 mm x 10 mm x 50 mm. 


![trilhomontado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/2f3b81c3-9a5f-49bd-84c4-c4f7e4e20c2d)

![20240522_105353 - Editado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/1ae7d759-14e0-4390-b23a-03aa221f68f2)
![20240522_105111 - Editado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/f1d993f5-63ca-4641-b090-bc4fdb1da175)
![20240522_103811 - Editado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/a34765de-bcf6-4930-bba8-d949ccbcc6f9)
![20240522_110341 - Editado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/471e90c7-8ddb-4416-a063-073ef16d23dc)



A rotina em python integrará a leitura do sensor de intensidade do smartphone e o comando da placa arduino uno. Para tanto o phyphox precisará ser ligado manualmente no 
smartphone, com permissão para acesso remoto. O endereço indicado no aplicativo precisará ser modificado na rotina do python.

![esquema-experimental (2)](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/f5f0de91-7234-472b-bb2b-0ae5d5039101)

A rotina funciona em quatro passos: comando para ligar o led em varredura e leitura do sinal produzido no smartphone para três condições, sem cubeta, com cubeta e solvente e com cubeta e amostra. O quarto passo integraliza as informações e apresenta o espectro. Os arquivos de base e o arquivo gerado na etapa quatro são salvos em uma pasta de referência. Na rotina original foi criada a pasta "dados", mas o usuário poderá customizar tanto o caminho quanto o nome da pasta no endereço dentro da rotina.


