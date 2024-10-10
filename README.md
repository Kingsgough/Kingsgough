<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Das Königsspiel Online</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 20px;
        }

        header {
            background: #333;
            color: #fff;
            padding: 10px 0;
            text-align: center;
        }

        h1, h2 {
            margin: 10px 0;
        }

        form {
            background: #fff;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        label {
            display: block;
            margin: 10px 0 5px;
        }

        input {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            background: #5cb85c;
            color: #fff;
            border: none;
            padding: 10px 15px;
            cursor: pointer;
            border-radius: 5px;
        }

        button:hover {
            background: #4cae4c;
        }

        footer {
            text-align: center;
            margin-top: 20px;
        }

        #taskList div {
            margin: 5px 0;
            padding: 10px;
            background: #e7f3fe;
            border: 1px solid #b3d4fc;
            border-radius: 4px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Willkommen zum Königsspiel Online!</h1>
    </header>
    
    <main>
        <section id="registration">
            <h2>Registrierung</h2>
            <form id="regForm">
                <label for="username">Benutzername:</label>
                <input type="text" id="username" name="username" required>
                
                <label for="email">E-Mail:</label>
                <input type="email" id="email" name="email" required>
                
                <label for="phone">Telefonnummer:</label>
                <input type="tel" id="phone" name="phone" required>
                
                <button type="submit">Registrieren</button>
            </form>
        </section>
        
        <section id="group-creation" style="display:none;">
            <h2>Gruppe erstellen</h2>
            <form id="groupForm">
                <label for="groupName">Gruppenname:</label>
                <input type="text" id="groupName" name="groupName" required>
                
                <button type="submit">Gruppe erstellen</button>
            </form>
        </section>
        
        <section id="tasks" style="display:none;">
            <h2>Aufgaben</h2>
            <div id="taskList"></div>
            <button id="nextTask">Nächste Aufgabe</button>
        </section>
    </main>
    
    <footer>
        <p>&copy; 2024 Das Königsspiel</p>
    </footer>

    <script>
        document.getElementById('regForm').addEventListener('submit', function(e) {
            e.preventDefault();
            document.getElementById('registration').style.display = 'none';
            document.getElementById('group-creation').style.display = 'block';
        });

        document.getElementById('groupForm').addEventListener('submit', function(e) {
            e.preventDefault();
            document.getElementById('group-creation').style.display = 'none';
            document.getElementById('tasks').style.display = 'block';
            loadTasks();
        });

        function loadTasks() {
            const tasks = [
                "Lass einen Mitspieler dir ein Strafelement anbringen.",
                "Mach ein peinliches Foto von dir und teile es in der Gruppe.",
                "Schicke einer Person in deinem Kontaktverzeichnis eine Nachricht, die du nicht senden würdest.",
                "Verrate einem Mitspieler ein Geheimnis über einen anderen."
            ];
            const taskList = document.getElementById('taskList');
            taskList.innerHTML = tasks.map(task => `<div>${task}</div>`).join('');
        }

        document.getElementById('nextTask').addEventListener('click', function() {
            // Hier kannst du die Logik für die nächste Aufgabe hinzufügen
            alert("Hier könnte deine nächste Aufgabe stehen!");
        });
    </script>
</body>
</html>
- 👋 Hi, I’m @Kingsgough
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Kingsgough/Kingsgough is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
