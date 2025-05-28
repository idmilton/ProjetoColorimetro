# Projeto Colorímetro

Projeto de construção e montagem de um colorímetro utilizando um led RGB, um smartphone, uma placa arduino e um código em python.
As peças para o trilho foram desenhadas e os desenhos em formato stl estão disponíveis para a reprodução. A montagem do trilho precisa ser complementada com 
hastes de aço de 1/4 de polegada e porcas compatíveis. O projeto utiliza um LED RGB alto brilho anodo comum tipo cápsula de 5 mm. Resistores precisam ser ligados
aos contatos do LED da sequinte forma: Contato do LED vermelho - 150 Ôhms, Contato do LED verde- 120 Ôhms e Contato do LED azul - 150 Ôhms. Eventualmente utilizando resistores de resistência um pouco menor poderá funcionar com tensão ainda anterior ao limiar dos LEDs. No trabalho de referência, foi utilizada uma cubeta de vidro comum, adquirida por 35 reais de 10 mm x 10 mm x 50 mm. 

# Colorimeter Project
Project to build and assemble a colorimeter using an RGB LED, a smartphone, an Arduino board and Python code.
The parts for the track have been designed and the drawings in stl format are available for reproduction. The rail assembly needs to be complemented with 
1/4 inch steel rods and compatible nuts. The project uses a 5 mm capsule-type common anode high-brightness RGB LED. Resistors need to be connected
to the LED contacts as follows: Red LED contact - 150 Ohms, Green LED contact - 120 Ohms and Blue LED contact - 150 Ohms. Eventually, using resistors with slightly lower resistance may work with voltages even lower than the LED threshold. In the reference work, a common glass cuvette was used, purchased for 35 reais measuring 10 mm x 10 mm x 50 mm.

![trilhomontado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/2f3b81c3-9a5f-49bd-84c4-c4f7e4e20c2d)

![20240522_105353 - Editado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/1ae7d759-14e0-4390-b23a-03aa221f68f2)
![20240522_105111 - Editado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/f1d993f5-63ca-4641-b090-bc4fdb1da175)
![20240522_103811 - Editado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/a34765de-bcf6-4930-bba8-d949ccbcc6f9)
![20240522_110341 - Editado](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/471e90c7-8ddb-4416-a063-073ef16d23dc)



A rotina em python integrará a leitura do sensor de intensidade do smartphone e o comando da placa arduino uno. Para tanto o phyphox precisará ser ligado manualmente no 
smartphone, com permissão para acesso remoto. O endereço indicado no aplicativo precisará ser modificado na rotina do python. A rotina funciona em quatro passos: comando para ligar o led em varredura e leitura do sinal produzido no smartphone para três condições, sem cubeta, com cubeta e solvente e com cubeta e amostra. O quarto passo integraliza as informações e apresenta o espectro. Os arquivos de base e o arquivo gerado na etapa quatro são salvos em uma pasta de referência. Na rotina original foi criada a pasta "dados", mas o usuário poderá customizar tanto o caminho quanto o nome da pasta no endereço dentro da rotina.

The Python routine will integrate the reading from the smartphone's intensity sensor and the command from the Arduino Uno board. To do so, phyphox will need to be manually connected to the smartphone, with permission for remote access. The address indicated in the application will need to be modified in the Python routine. The routine works in four steps: command to turn on the scanning LED and reading of the signal produced on the smartphone for three conditions, without cuvette, with cuvette and solvent and with cuvette and sample. The fourth step integrates the information and presents the spectrum. The base files and the file generated in step four are saved in a reference folder. In the original routine, the "data" folder was created, but the user can customize both the path and the name of the folder in the address within the routine.

![esquema-experimental (2)](https://github.com/idmilton/ProjetoColorimetro/assets/4228326/f5f0de91-7234-472b-bb2b-0ae5d5039101)


Referência: https://www.scielo.br/j/rbef/a/jqWKDMpTVzzQGYtcdVswTTc/?format=pdf&lang=pt

