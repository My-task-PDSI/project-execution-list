
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
  - [**rota GET grupo-tarefas/all/**](#rotaGETgrupotarefasall)
  - [**rota GET grupo-tarefas/:id/**](#rotaGETgrupotarefasid)
  - [**rota POST tarefas/add/**](#rotaPOSTtarefasadd)
  - [**rota GET grupo-tarefas/all/**](#rotaGETgrupotarefasall)


## BACKEND

## <a name="Configuraçãoinicialserver"><a> Configuração inicial server 
##### [voltar ao topo](#sumario)
+ [X] Criar o servidor( apenas o basico para execução)
+ [ ] Criar rotas para teste de funcionamento

## <a name="Configuraçãoinicialdatabase"> Configuração inicial database
##### [voltar ao topo](#sumario)
+ [X] Criar banco de dados
+ [X] Conectar banco de dados

## <a name="Criartabelas"> Criar tabelas
##### [voltar ao topo](#sumario)
- [X] Criar tabela Usuario
- [X] Criar tabela Grupo de tarefa
- [X] Criar tabela Tarefa
- [X] Criar tabela Notificação( opcional , pode ficar por ultimo)

## <a name="Criaçãodasrotasiniciais"> Criação das rotas iniciais
##### [voltar ao topo](#sumario)
- [ ] Criar rota para manipulção de usuarios
- [ ] Criar rota para manipulção de grupos de tarefas
- [ ] Criar rota para manipulção de tarefas
- [ ] Criar rota para manipulção de notificação

## <a name="Rotausuario"> Rota usuario
##### [voltar ao topo](#sumario)
- [ ] criar crud para usuario

## <a name="RotaGrupodetarefa"> Rota Grupo de tarefa
##### [voltar ao topo](#sumario)
- [ ] criar crud para grupo de tarefas
- [ ] criar rota que devolve todos os grupos de um usuario
- [ ] criar rota que devolve um grupo e todas suas tarefas

## <a name="RotaTarefa"> Rota Tarefa
##### [voltar ao topo](#sumario)
- [ ] criar crud para tarefa

# <a name="Formatodedevoluçãoparaalgumasrotas"> Formato de devolução para algumas rotas

## <a name="rotaGETgrupotarefasall"> rota GET grupo-tarefas/all/
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

## <a name="rotaGETgrupotarefasid"> rota GET grupo-tarefas/:id/
##### [voltar ao topo](#sumario)
recebe:

**params**:
+ id : id grupo

**body**:
+ N/A

retorna:

```json
{
    "grupo": "{...info_grupo}",
    "tarefas": [
        "{...info_tarefa_1}",
        "{...info_tarefa_2}",
        "{...info_tarefa_N}"
    ],
}
```

## <a name="rotaPOSTtarefasadd"> rota POST tarefas/add/
##### [voltar ao topo](#sumario)
recebe:

**params**:
+ N/A

**body**:

```json
{
    "body": {
        "id_grupo":"id",
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


