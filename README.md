# audima

Passo a passo para executar a aplicação

- Backend Laravel
  - Na pasta audimaLaravel, crie o arquivo .env
  - Na pasta audimaLaravel, execute o comando "composer install"
  - Definr o host, login e senha no .env
	- Criar o banco 'audima'
	- Como não criei migrations e nem seeder, executar o arquivo audimaSql.sql no mysql
	- Criar o virtual host http://audima.test, pois o angular usa esse endereço
	- No projeto laravel, na pasta audimaLaravel é só usar o comando "php artisan crawler:start" para executar o robo
	
- Frontend Angular
	- No projeto Angular, na pasta angularAudima. O endereço da API de consulta esta definido no arquivo:
	audimaAngular\src\app\app.component.ts, na variável url = 'http://audima.test/get/dados'; que esta na linha 13
	Caso seja definido um endereço diferente no projeto laravel, esse novo endereço deverá ser atualizado nessa variável url da linha 13
	- NO projeto Angular, na pasta angularAudima é só executar o comando "ng serve --open" para exibir a aplicação
	
	