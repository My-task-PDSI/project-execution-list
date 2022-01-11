
# Lista de funcionalidades e tarefas a serem completadas pelo frontend

## <a name="sumario"><a> Sumario

+ [**Configuração inicial do frontend**](#Configuraçaoinicialdofront)
+ [**Configuração de database fake**](#Configuraçãodedatabasefake)
+ [**Criar rotas**](#Criarrotas)
+ [**Login**](#Login)
+ [**Grupo de tarefa**](#Grupo)
+ [**Tarefa**](#Tarefa)
+ [**Formato para algumas rotas**](#FormatoRotas)


## FRONTEND

## <a name="Configuraçaoinicialdofront"><a> Configuração inicial do frontend
+ [x] Criar o servidor( apenas o basico para execução)
+ [x] Criar rotas para teste de funcionamento

## <a name="Configuraçãodedatabasefake"> Configuração de database fake
+ [x] instalar json-server
+ [x] testar e criar rotas

## <a name="Criarrotas"> Criar rotas
##### [voltar ao topo](#sumario)
- [x] Criar rota para manipulção de usuarios
- [x] Criar rota para manipulção de grupos de tarefas
- [x] Criar rota para manipulção de tarefas
- [x] Criar rota para manipulção de notificação

## <a name="Login"> Login
##### [voltar ao topo](#sumario)
- [x] criar tela de login
- [x] criar criar tela de cadastro
- [x] adicionar eventos(fetch de dados/etc)

## <a name="Grupo"> Grupo de tarefa
##### [voltar ao topo](#sumario)
- [x] criar tela de listagem de grupo de tarefas
- [x] criar tela de crud de grupo de tarefas
- [x] implementar a listagem de tarefas na tela anterior

## <a name="Tarefa"> Tarefa
##### [voltar ao topo](#sumario)
- [x] criar card para tarefa
- [x] cada card pode ser responsivo contendo o proprio sistema
de crud nele ou pode criar uma tela apenas para edicao dessa tarefa

## <a name="integraçãoBackend"> integração com o backend
##### [voltar ao topo](#sumario)
- [x] conectar sistema de login ao back
- [x] conectar sistema de cadastro ao back
- [x] conectar sistema de listagem de grupo ao back
- [x] conectar sistema de crud do grupo e tarefas com o back

# <a name="formatoRotas"> Formato para algumas rotas
##### [voltar ao topo](#sumario)

+ **login**:
  - user/login/
+ **cadastro**:
  - user/singup/
+ **grupos de tarefa**:
  - task-groups/
+ **grupo de tarefa especifico/tela do crud de grupos**:
  - task-groups/**:idGrupo**/
+ **tela de crud tarefa especifica**(caso seja implementada):
  - task/**:idTarefa**/


