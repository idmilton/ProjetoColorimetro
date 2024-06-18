# ProjetoColorimetro
Projeto de construção e montagem de um colorímetro utilizando um led RGB, um smartphone, uma placa arduino e um código em python.
As peças para o trilho foram desenhadas e os desenhos em formato stl estão disponíveis para a reprodução. A montagem do trilho precisa ser complementada com 
hastes de aço de 1/4 de polegada e porcas compatíveis. O projeto utiliza um LED RGB alto brilho anodo comum tipo cápsula de 5 mm. Resistores precisam ser ligados
aos contatos do LED da sequinte forma: Contato do LED vermelho - 150 Ôhms, Contato do LED verde- 120 Ôhms e Contato do LED azul - 150 Ôhms. Eventualmente utilizando resistores de resistência um pouco menor poderá funcionar com tensão ainda anterior ao limiar dos LEDs. No trabalho de referência, foi utilizada uma cubeta de vidro comum, adquirida por 35 reais de 10 mm x 10 mm x 50 mm. 


![trilhomontado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/2f3b81c3-9a5f-49bd-84c4-c4f7e4e20c2d)

![20240522_103811](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/b081db80-440b-432b-8dda-4dc649fbdc88)
![20240522_110341](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/f1e68967-db44-45ae-98b8-d545fc2acc4d)
![20240522_105353](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/1499ea80-f8d1-429e-b712-4f73a106f1ff)
![20240522_105111](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/e5d0f797-1ecf-4ed9-aa4e-962db04e78f2)


A rotina em python integrará a leitura do sensor de intensidade do smartphone e o comando da placa arduino uno. Para tanto o phyphox precisará ser ligado manualmente no 
smartphone, com permissão para acesso remoto. O endereço indicado no aplicativo precisará ser modificado na rotina do python.

![esquema-experimental (2)](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/f5f0de91-7234-472b-bb2b-0ae5d5039101)

A rotina funciona em quatro passos: comando para ligar o led em varredura e leitura do sinal produzido no smartphone para três condições, sem cubeta, com cubeta e solvente e com cubeta e amostra. O quarto passo integraliza as informações e apresenta o espectro. Os arquivos de base e o arquivo gerado na etapa quatro são salvos em uma pasta de referência. Na rotina original foi criada a pasta "dados", mas o usuário poderá customizar tanto o caminho quanto o nome da pasta no endereço dentro da rotina.


