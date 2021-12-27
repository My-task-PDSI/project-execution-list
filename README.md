# project-execution-list
repo com as principais coisas a serem feitas

# Lista de funcionalidades e tarefas a serem completadas

## Sumario

+ [**Configuração inicial server**](#Configuraçãoinicialserver)
+ [**Configuração inicial database**](#Configuraçãoinicialdatabase)
+ [**Criar tabelas**](#Criartabelas)
+ [**Criação das rotas iniciais**](#Criaçãodasrotasiniciais)
+ [**Rota usuario**](#Rotausuario)
+ [**Rota Grupo de tarefa**](#RotaGrupodetarefa)
+ [**Rota Tarefa**](#RotaTarefa)
+ [**Formato de devolução para algumas rotas**](#Formatodedevoluçãoparaalgumasrotas)
  - [**rota GET grupo-tarefas/all/**](#rotaGETgrupotarefasall)
  - [**rota GET grupo-tarefas/:id/**](#rotaGETgrupotarefasid)
  - [**rota POST tarefas/add/**](#rotaPOSTtarefasadd)
  - [**rota GET grupo-tarefas/all/**](#rotaGETgrupotarefasall)


## BACKEND

## <a name="Configuraçãoinicialserver"><a> Configuração inicial server 
+ [ ] Criar o servidor( apenas o basico para execução)
+ [ ] Criar rotas para teste de funcionamento

## <a name="Configuraçãoinicialdatabase"> Configuração inicial database
+ [ ] Criar banco de dados
+ [ ] Conectar banco de dados

## <a name="Criartabelas"> Criar tabelas
- [ ] Criar tabela Usuario
- [ ] Criar tabela Grupo de tarefa
- [ ] Criar tabela Tarefa
- [ ] Criar tabela Notificação( opcional , pode ficar por ultimo)

## <a name="Criaçãodasrotasiniciais"> Criação das rotas iniciais
- [ ] Criar rota para manipulção de usuarios
- [ ] Criar rota para manipulção de grupos de tarefas
- [ ] Criar rota para manipulção de tarefas
- [ ] Criar rota para manipulção de notificação

## <a name="Rotausuario"> Rota usuario
- [ ] criar crud para usuario

## <a name="RotaGrupodetarefa"> Rota Grupo de tarefa
- [ ] criar crud para grupo de tarefas
- [ ] criar rota que devolve todos os grupos de um usuario
- [ ] criar rota que devolve um grupo e todas suas tarefas

## <a name="RotaTarefa"> Rota Tarefa
- [ ] criar crud para tarefa

# <a name="Formatodedevoluçãoparaalgumasrotas"> Formato de devolução para algumas rotas

## <a name="rotaGETgrupotarefasall"> rota GET grupo-tarefas/all/
recebe:

**params**:
+ N/A

**body**:
+ N/A ou alguma info de usuario

retorna:

```json
{
    /*pode ser todas as info ou somente id+titulo*/
    'grupos': [
        {...info_grupo_1},
        {...info_grupo_2},
        {...info_grupo_N}
    ],
}
```

## <a name="rotaGETgrupotarefasid"> rota GET grupo-tarefas/:id/
recebe:

**params**:
+ id : id grupo

**body**:
+ N/A

retorna:

```json
{
    'grupo': {...info_grupo},
    'tarefas': [
        {...info_tarefa_1},
        {...info_tarefa_2},
        {...info_tarefa_N}
    ],
}
```

## <a name="rotaPOSTtarefasadd"> rota POST tarefas/add/
recebe:

**params**:
+ N/A

**body**:

```json
{
    'body': {
        'id_grupo':'id',
        'tarefa':{...info_tarefa},
    }
}
```
retorna:

```json
{
    /*dados da tarefa adicionada + id*/
    'tarefa': {...info_tarefa_criada},
    /*opcional*/
    'error': {
        'mensagem':'mensagem',
    },
}
```


