# artisan-list
## Comandos mais usados Laravel

Listagem de comandos do artisan 
Abaixo irei listar a maioria (se não todos) os comandos para o artisan, também deixarei pequenos exemplos e informações para que servem cada um deles.

php artisan clear-compiled
Remove os arquivos de classe já compilados.

php artisan down
Coloca aplicação em modo de manutenção.

php artisan up
Tira a aplicação de modo de manutenção e coloca novamente em produção. 

php artisan env
Exibe as variáveis de ambiente definidas para o framework, por exemplo se está é uma aplicação local ou está no servidor.

php artisan help
Exibe a ajuda para os comandos determinados.

php artisan list
Exibe a listagem de comandos disponíveis.

php artisan migrate
Executa as migrations de um banco de dados, esse comando recebe alguns outros parâmetros e vamos vê-los.

php artisan migrate:install
Cria a tabela migrations, e caso já exista exibe um erro pois a tabela já foi criada, quando realizado o migrate essa tabela também é criada automaticamente.

php artisan migrate:refresh
Redefine e reexecuta todas as migrations.

php artisan migrate:reset
Desfaz todas as ações executadas pelas migratórios.

php artisan migrate:rollback
Desfaz a última ação executada pela migration.

php artisan migrate:status
Exibe o status de cada migration, (Y para as executadas e N para não executadas).

php artisan optimize
Otimiza o framework para uma melhor performance.

php artisan tinker
Torna os comandos do artisan interativos, quando executado entra em modo de terminal, assim podendo executar classes e também podendo executar todos os comandos do artisan sem a necessidade de colocar o "php artisan".

php artisan app:name
Redefine o namespace da aplicação, (por padrão é o App).

php artisan auth:clear-resets 
Remove os tokens expirados de renovação de senhas

php artisan cache:clear
Limpa o cache da aplicação

php artisan cache:table
Cria uma migração para a tabela cache do banco de dados.

php artisan config:cache
Cria um arquivo de cache para acelerar o acesso dos dados de configuração, quando executado ele antes de criar realizar o comando config:clear.

php artisan config:clear
Remove o arquivo de cache criado para acelerar o acesso dos dados de configuração.

php artisan db:seed
executa o processo de seed do banco de dados, caso queria definir uma seed específica basta passar o parâmetro --class=NomeDaClasse, exemplo:
php artisan db:seed --class=SeedDatabaseFeliz.

php artisan event:generate
Gera os eventos e registros ausentes baseado em seus registros, (tradução), ao executar esse comando ele criou algumas classes (App\Events\Event; e App\Listeners\EventsListeners) ainda não sei bem o que é mais descobrindo atualizarei aqui!

php artisan key:generate
Gera uma chave para aplicação, quando realizado a instalação do Laravel essa chave já é criada no arquivo .env, sendo basicamente usada quando realizado um pull de algum repositório.

php artisan make:auth
Gera um scaffold(andaime) de login, isso é cria todas as camadas necessárias para realização de cadastro login e recuperação de senha.

php artisan make:command [NomeClasse]
Cria uma nova classe de comando para o artisan, localizada em app/Console/Commands/NomeClase.php.

php artisan make:controller [NomeClasse]
Gera um novo Controller, localizado em app/Http/Controllers/NomeClasse.php.

php artisan make:event [NomeClasse]
Gera uma nova classe do tipo Evento, localizado em app/Events/NomeClasse.php.

php artisan make:job [NomeClasse]
Gera uma nova classe do tipo Job, localizado em app/Jobs/NomeClasse.php.

php artisan make:listener [NomeClasse]

Gera uma classe do tipo Listener relacionado a algum evento.

php artisan make:mail [NomeClasse]
Gera uma classe do tipo E-mail, localizado em app/Mail/NomeClasse.php.

php artisan make:middleware [NomeClase]
Gera uma classe do tipo middleware, localizada em app/Http/Middleware/NomeClasse.php.

php artisan make:migration [NomeClasse]
Gera uma nova classe do tipo migration, localizada em database/migrations/NomeClasse.php.

php artisan make:notification [NomeClasse]
Gera uma nova classe do tipo notification, logalizada em app/Notifications/NomeClasse.php

php artisan make:policy [NomeClasse]
Gera uma nova classe do tipo policy, localizada em app/Policies/NomeClasse.php

php artisan make:provider [NomeClasse]
Gera uma nova classe do tipo provider, localizada em app/Providers/NomeClasse.php

php artisan make:request  [NomeClasse]
Gera uma nova classe do tipo request, localizada em app/Http/Requests/NomeClasse.php
 
php artisan make:seeder [NomeClasse]
Gera uma nova classe do tipo seed responsável por popular a tabela, se localiza em app/database/seeds/NomeClasse.php
 
php artisan make:test [NomeClasse]
Gera uma nova classe do tipo teste, as quais normalmente são executadas pelo phpUnit localizando em vendor/phpunit, a classe gerada se localiza em /tests.

php artisan queue:failed
Lista todos os jobs (tarefas) com falha em uma fila.

php artisan queue:failed-table
Cria uma migration para a tabela "failed_jobs".

php artisan queue:flush

Limpa todos os trabalhos com falha em uma fila.

php artisan queue:forget
Exclui uma tarefa com falha da fila.

php artisan queue:listen
"Escuta" uma fila em execução.

php artisan queue:restart
Reinicia o processamento de uma fila.

php artisan queue:retry
Submete novamente uma fila com falhas para execução.

php artisan queue:table
Cria uma classe de migration para uma determinada fila,

php artisan queue:work
Executa a próxima tarefa de uma fila. 

php artisan route:cache
Cria um arquivo de cache para as rotas

php artisan route:clear
Limpa o arquivo de cache das rotas

php artisan route:list
Lista todas as rotas da aplicação

php artisan schedule:run
Executa comandos agendados

php artisan session:table
Cria uma migration para os dados de sessão.

php artisan storage:link
Cria um link simbólico de public/storage para storage/app/public.

php artisan vendor:publish
Publica arquivos públicos de pacotes de terceiros.

php artisan view:clear
Limpa os arquivos compilados das views.
