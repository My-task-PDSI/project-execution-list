
# Lista de funcionalidades e tarefas a serem completadas pelo backend

## <a name="sumario"><a> Sumario

+ [**Configuração inicial server**](#Configuraçãoinicialserver)
+ [**Configuração inicial database**](#Configuraçãoinicialdatabase)
+ [**Criar tabelas**](#Criartabelas)
+ [**Criação das rotas iniciais**](#Criaçãodasrotasiniciais)
+ [**Rota usuario**](#Rotausuario)
+ [**Rota Grupo de tarefa**](#RotaGrupodetarefa)
+ [**Rota Tarefa**](#RotaTarefa)
+ [**Formato de devolução para algumas rotas**](#Formatodedevoluçãoparaalgumasrotas)
  - [**rota GET task-groups/all/**](#rotaGETgrupotarefasall)
  - [**rota GET task-groups/:id/**](#rotaGETgrupotarefasid)
  - [**rota POST tasks/**](#rotaPOSTtarefasadd)
  - [**rota GET task-groups/all/**](#rotaGETgrupotarefasall)


## BACKEND

## <a name="Configuraçãoinicialserver"><a> Configuração inicial server 
##### [voltar ao topo](#sumario)
+ [x] Criar o servidor( apenas o basico para execução)
+ [x] Criar rotas para teste de funcionamento

## <a name="Configuraçãoinicialdatabase"> Configuração inicial database
##### [voltar ao topo](#sumario)
+ [x] Criar banco de dados
+ [x] Conectar banco de dados

## <a name="Criartabelas"> Criar tabelas
##### [voltar ao topo](#sumario)
- [x] Criar tabela Usuario
- [x] Criar tabela Grupo de tarefa
- [x] Criar tabela Tarefa
- [x] Criar tabela Notificação( opcional , pode ficar por ultimo)

## <a name="Criaçãodasrotasiniciais"> Criação das rotas iniciais
##### [voltar ao topo](#sumario)
- [x] Criar rota para manipulção de usuarios
- [x] Criar rota para manipulção de grupos de tarefas
- [x] Criar rota para manipulção de tarefas
- [x] Criar rota para manipulção de notificação

## <a name="Rotausuario"> Rota usuario
##### [voltar ao topo](#sumario)
- [x] criar crud para usuario

## <a name="RotaGrupodetarefa"> Rota Grupo de tarefa
##### [voltar ao topo](#sumario)
- [x] criar crud para grupo de tarefas
- [x] criar rota que devolve todos os grupos de um usuario
- [x] criar rota que devolve um grupo

## <a name="RotaTarefa"> Rota Tarefa
##### [voltar ao topo](#sumario)
- [x] criar rota que devolve todas suas tarefas de um grupo
- [x] criar crud para tarefa

# <a name="Formatodedevoluçãoparaalgumasrotas"> Formato de devolução para algumas rotas

## <a name="rotaGETgrupotarefasall"> rota GET task-groups/all/
##### [voltar ao topo](#sumario)
recebe:

**params**:
+ N/A

**body**:
+ N/A ou alguma info de usuario

retorna:

```json
{
    
    "grupos": [
        "{...info_grupo_1}",
        "{...info_grupo_2}",
        "{...info_grupo_N}"
    ],
}
```

## <a name="rotaGETgrupotarefasid"> rota GET task-groups/:id/
##### [voltar ao topo](#sumario)
recebe:

**params**:
+ id : id grupo

**body**:
+ N/A

retorna:

```json
{
    "tarefas": [
        "{...info_tarefa_1}",
        "{...info_tarefa_2}",
        "{...info_tarefa_N}"
    ],
}
```

## <a name="rotaPOSTtarefasadd"> rota POST tasks/
##### [voltar ao topo](#sumario)
recebe:

**params**:
+ N/A

**body**:

```json
{
    "body": {
        "tarefa":"{...info_tarefa}",
    }
}
```
retorna:

```json
{
    
    "tarefa": "{...info_tarefa_criada}",
    "error": {
        "mensagem":"mensagem",
    },
}
```


