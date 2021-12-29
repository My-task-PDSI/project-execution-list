
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
- [ ] Criar rota para manipulção de usuarios
- [x] Criar rota para manipulção de grupos de tarefas
- [ ] Criar rota para manipulção de tarefas
- [ ] Criar rota para manipulção de notificação

## <a name="Login"> Login
##### [voltar ao topo](#sumario)
- [ ] criar tela de login
- [ ] criar criar tela de cadastro
- [ ] adicionar eventos(fetch de dados/etc)

## <a name="Grupo"> Grupo de tarefa
##### [voltar ao topo](#sumario)
- [ ] criar tela de listagem de grupo de tarefas
- [ ] criar tela de crud de grupo de tarefas
- [ ] implementar a listagem de tarefas na tela anterior

## <a name="Tarefa"> Tarefa
##### [voltar ao topo](#sumario)
- [ ] criar card para tarefa
- [ ] cada card pode ser responsivo contendo o proprio sistema
de crud nele ou pode criar uma tela apenas para edicao dessa tarefa

## <a name="integraçãoBackend"> integração com o backend
##### [voltar ao topo](#sumario)
- [ ] conectar sistema de login ao back
- [ ] conectar sistema de cadastro ao back
- [ ] conectar sistema de listagem de grupo ao back
- [ ] conectar sistema de crud do grupo e tarefas com o back

# <a name="formatoRotas"> Formato para algumas rotas
##### [voltar ao topo](#sumario)

+ **login**:
  - login/
+ **cadastro**:
  - cadastro/
+ **grupos de tarefa**:
  - grupos-de-tarefa/
+ **grupo de tarefa especifico/tela do crud de grupos**:
  - grupos-de-tarefa/**:id_grupo**/
+ **tela de crud tarefa especifica**(caso seja implementada):
  - grupos-de-tarefa/tarefa/**:id_tarefa**/


