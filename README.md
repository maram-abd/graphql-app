json pour tester
1-récupérer les taches:
{
  "query": "query { tasks { id title description completed duration } }"
}
2-ajouter une tache:
{
  "query": "mutation { addTask(title: \"newtask\", description: \"desc task\", completed: false) { id title description completed } }"
}

3-supprimer une tache :
{
  "query": "mutation { deleteTask(id: \"4\") { id title description completed } }"
}

4-changer description:
{
  "query": "mutation { changeDescription(id: \"5\", newDescription: \"new description\") { id title description completed } }"
}

5-tache complete:
{
  "query": "mutation { completeTask(id: \"5\") { id title description completed } }"
}

6-récupérer une tache spécifique:
{
  "query": "{ task(id: \"3\") { id title description completed } }"
}
