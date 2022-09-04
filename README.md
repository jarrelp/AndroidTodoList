# AndroidTodoList

activity_main.xml:
    maak layout van de main activity screen
    met recyclerview die gebruikt wordt om de todoitems weer te geven

item_todo.xml:
    maak layout van elke todoitem

Todokt:
    tododata class

Todoadapterclass:
    bevat de behaviour van de todolist

    TodoViewHolder:
        class is gewrapped om een speciafieke view
        de view in dit geval is de constraintlayout (rootlayout) in item_todo.xml
        hiermee wordt alleen de items geladen die geladen moeten worden (performanceboost)

    oncreateviewholder:
        hier wordt de viewholder geretoneert
        de layoutInflater zorgt ervoor dat de item_todo.xml gelezen kan worden in Kotlin

    onBindViewHolder:
        zet de data van de todolist naar de textview en checkbox van de specifieke item


    getItemFunction:
        zorgt ervoor dat de recycler weet hoeveel items er in de todolist zitten

    toggleStrikeThrough:
        helper function is gemaakt om de behaviour van het togglen van een textvield te specificeren

    deleteDoneTodos:
        helper function is gemaakt om de behaviour van het deleten van de done todos te specifieren
        met een notificatie

    addTodo:
        helper function is gemaakt om de behaviour van het aanmaken van een todox te specifieren
        met een notificatie

MainActivity:
    create function wordt aangeroepen wanneer deze applicatie opgestart wordt
    recycleviewtodoitems.adapter krijgt todoadapter
    recycleviewtodoitems.layoutmanager krijgt linearLayoutManager(this)
    btnAddTodo.setOnClickListener
    btnDeleteDoneTodos.setOnClickListener


### ---> nog lastig te begrijpen wat er gedaan wordt met rvTodoItems <-- ###
