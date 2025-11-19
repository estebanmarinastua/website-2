<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Task Manager - CRUD</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f7f7f7;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .task-container {
            width: 400px;
            background-color: white;
            padding: 20px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
        .task-container h1 {
            text-align: center;
            margin-bottom: 20px;
        }
        .input-group {
            display: flex;
            margin-bottom: 20px;
        }
        .input-group input {
            flex: 1;
            padding: 10px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .input-group button {
            padding: 10px;
            font-size: 16px;
            margin-left: 10px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        .input-group button:hover {
            background-color: #45a049;
        }
        .task-list {
            list-style: none;
            padding: 0;
            margin: 0;
        }
        .task-list li {
            background-color: #f1f1f1;
            margin: 10px 0;
            padding: 10px;
            border-radius: 4px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .task-list li.completed {
            text-decoration: line-through;
            background-color: #d3ffd3;
        }
        .task-list li button {
            background-color: #f44336;
            color: white;
            border: none;
            border-radius: 4px;
            padding: 5px 10px;
            cursor: pointer;
        }
        .task-list li button:hover {
            background-color: #f33;
        }
        .task-list li .edit-btn {
            background-color: #ff9800;
            margin-right: 10px;
        }
        .task-list li .edit-btn:hover {
            background-color: #f57c00;
        }
        .task-list li input {
            flex: 1;
            font-size: 16px;
            padding: 5px;
            border: none;
            background: none;
        }
    </style>
</head>
<body>

    <div class="task-container">
        <h1>Task Manager - CRUD</h1>
        <div class="input-group">
            <input type="text" id="taskInput" placeholder="Nueva tarea...">
            <button onclick="addTask()">Agregar</button>
        </div>
        <ul id="taskList" class="task-list">
            <!-- Las tareas aparecerán aquí -->
        </ul>
    </div>

    <script>
        // Cargar tareas desde el localStorage
        window.onload = function() {
            loadTasks();
        };

        function loadTasks() {
            const taskList = JSON.parse(localStorage.getItem('tasks')) || [];
            const taskListContainer = document.getElementById('taskList');
            taskListContainer.innerHTML = '';  // Limpiar lista

            taskList.forEach((task, index) => {
                const li = document.createElement('li');
                li.classList.toggle('completed', task.completed);
                li.innerHTML = `
                    <input type="text" value="${task.name}" onblur="updateTask(${index}, this.value)" onclick="editTask(this)">
                    <button class="edit-btn" onclick="toggleTaskStatus(${index})">Completado</button>
                    <button onclick="removeTask(${index})">Eliminar</button>
                `;
                taskListContainer.appendChild(li);
            });
        }

        function addTask() {
            const taskInput = document.getElementById('taskInput');
            const taskValue = taskInput.value.trim();

            if (taskValue === '') {
                alert('Por favor ingresa una tarea.');
                return;
            }

            const taskList = JSON.parse(localStorage.getItem('tasks')) || [];
            const newTask = { name: taskValue, completed: false };

            taskList.push(newTask);
            localStorage.setItem('tasks', JSON.stringify(taskList));
            taskInput.value = '';  // Limpiar campo
            loadTasks();
        }

        function toggleTaskStatus(index) {
            const taskList = JSON.parse(localStorage.getItem('tasks')) || [];
            taskList[index].completed = !taskList[index].completed;
            localStorage.setItem('tasks', JSON.stringify(taskList));
            loadTasks();
        }

        function removeTask(index) {
            const taskList = JSON.parse(localStorage.getItem('tasks')) || [];
            taskList.splice(index, 1);
            localStorage.setItem('tasks', JSON.stringify(taskList));
            loadTasks();
        }

        function editTask(inputElement) {
            inputElement.select(); // Selecciona el texto al hacer clic
        }

        function updateTask(index, newName) {
            const taskList = JSON.parse(localStorage.getItem('tasks')) || [];
            if (newName.trim() !== '') {
                taskList[index].name = newName.trim();
                localStorage.setItem('tasks', JSON.stringify(taskList));
            }
            loadTasks();
        }
    </script>

</body>
</html>
