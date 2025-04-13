# Al-junaid-tech-WebDevTask3
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home - My Website</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="style.css">
    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>
</head>
<body>

    <header>
        <nav class="navbar navbar-expand-lg  ">
            <a class="navbar-brand" href="index.html">BLOOMIX<br><h6>    By Mishal</h6></a>
            
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ml-auto">
                    <li class="nav-item active"><a class="nav-link" href="index.html">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="about.html">About Us</a></li>
                    <li class="nav-item"><a class="nav-link" href="contact.html">Contact Us</a></li>
                    <li class="nav-item"><a class="nav-link" href="register.html">Registration</a></li>
                    <li class="nav-item"><a class="nav-link" href="login.html">Login</a></li>
                    <li class="nav-item"><a class="nav-link" href="todo.html">To-Do List</a></li>

                </ul>
            </div>
        </nav>
    </header>

    <main class="container mt-4 fade-in">
        <h1 style="color: rgb(255, 255, 255);">Welcome to BLOOMIX!</h1>
        <div class="bird">
        
        <p ><br>Welcome! We specialize in crafting modern, responsive, and user-friendly websites.<br> Explore our services and let's bring your vision to life.</p>
        <img src="flying-7288_256.gif" alt="">
    </div>
        <div class="intro" >
          
        
        <div class="aboutus">
            <div class="about"><img src="w1pg.jpg" alt=""></div>
            <div class="about"><img src="w2pg.jpg" alt=""></div>
            <div class="about"><img src="w3pg.jpg" alt=""></div>
            <div class="about"><img src="wpg.jpg" alt=""></div>
        </div>
        
    </div>
    </main>


    <footer class="bg-light text-center py-3">
        <p>&copy; 2024 My Website. All rights reserved.</p>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.3/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    <script src="script.js"></script>
    <!-- To-Do List Modal -->
<div class="modal fade" id="todoModal" tabindex="-1" aria-labelledby="todoModalLabel" aria-hidden="true">
    <div class="modal-dialog modal-lg">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="todoModalLabel">To-Do List</h5>
          <button type="button" class="close" data-dismiss="modal" aria-label="Close">
            <span>&times;</span>
          </button>
        </div>
        <div class="modal-body">
          <!-- Task Form -->
          <form id="taskForm">
            <div class="form-group">
              <label for="taskTitle">Title</label>
              <input type="text" class="form-control" id="taskTitle" required>
            </div>
            <div class="form-group">
              <label for="taskDescription">Description</label>
              <textarea class="form-control" id="taskDescription" rows="3" required></textarea>
            </div>
            <input type="hidden" id="editIndex">
            <button type="submit" class="btn btn-primary">Save Task</button>
          </form>
          <hr>
          <!-- Task List -->
          <ul class="list-group" id="taskList"></ul>
        </div>
      </div>
    </div>
  </div>
  
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home - My Website</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="style.css">
    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>
</head>
<body>
    <header>
        <nav class="navbar navbar-expand-lg  ">
            <a class="navbar-brand" href="index.html">BLOOMIX<br><h6>    By Mishal</h6></a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ml-auto">
                    <li class="nav-item active"><a class="nav-link" href="index.html">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="about.html">About Us</a></li>
                    <li class="nav-item"><a class="nav-link" href="contact.html">Contact Us</a></li>
                    <li class="nav-item"><a class="nav-link" href="register.html">Registration</a></li>
                    <li class="nav-item"><a class="nav-link" href="login.html">Login</a></li>
                    <li class="nav-item"><a class="nav-link" href="todo.html">To-Do List</a></li>
                </ul>
            </div>
        </nav>
    </header>

    <main class="container todo-container mt-4 fade-in">
        <div class="form-container">
            <h4>To-Do List</h4>
            <form id="taskForm">
                <div class="form-group">
                    <label>Task Title</label>
                    <input type="text" id="taskTitle" class="form-control" required>
                </div>
                <div class="form-group">
                    <label>Task Description</label>
                    <textarea id="taskDescription" class="form-control" rows="3" required></textarea>
                </div>
                <input type="hidden" id="editIndex">
                <button type="submit" class="btn btn-dark">Add Task</button>
            </form>
            <hr>

            <ul id="taskList" class="list-group mt-3"></ul>
        </div>
    </div>
</div>
        </div>
    </main>
    <!-- Scripts -->
    <script>
        const taskForm = document.getElementById('taskForm');
        const taskList = document.getElementById('taskList');
        let tasks = JSON.parse(localStorage.getItem('tasks')) || [];

        const renderTasks = () => {
            taskList.innerHTML = '';
            tasks.forEach((task, index) => {
                const li = document.createElement('li');
                li.className = 'list-group-item custom-task-item d-flex justify-content-between align-items-center flex-column flex-sm-row';

                li.innerHTML = `
                    <div>
                        <strong>Title<br>${task.title}</strong>
                        <strong><br>Description<br></strong><small>${task.description}</small>
                    </div>
                    <div class="mt-2 mt-sm-0">
                        <button class="btn btn-sm btn-dark mr-2" onclick="editTask(${index})">Edit</button>
                        <button class="btn btn-sm btn-dark" onclick="deleteTask(${index})">Delete</button>
                    </div>
                `;
                taskList.appendChild(li);
            });
            localStorage.setItem('tasks', JSON.stringify(tasks));
        };

        taskForm.addEventListener('submit', function (e) {
            e.preventDefault();
            const title = document.getElementById('taskTitle').value.trim();
            const desc = document.getElementById('taskDescription').value.trim();
            const index = document.getElementById('editIndex').value;

            if (!title || !desc) return;

            if (index !== '') {
                tasks[index] = { title, description: desc };
            } else {
                tasks.push({ title, description: desc });
            }

            taskForm.reset();
            document.getElementById('editIndex').value = '';
            renderTasks();
        });

        function editTask(index) {
            const task = tasks[index];
            document.getElementById('taskTitle').value = task.title;
            document.getElementById('taskDescription').value = task.description;
            document.getElementById('editIndex').value = index;
        }

        function deleteTask(index) {
            tasks.splice(index, 1);
            renderTasks();
        }

        // Initial load
        renderTasks();
    </script>

</body>
</html>
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #1a1a1a;
    color: #e0e0e0;
    margin: 0;
    padding: 0;
    background-image: url(1.jpg);
    background-size: cover;
}

header, footer {
    background-color:rgb(0, 0, 0);;
}

.nav-link {
    color: whitesmoke !important;
    transition: color 1.6s ease;
    font-size: medium;
}

.nav-link:hover {
    color: rgb(160, 1, 252) !important;
}

.navbar-brand {
    color: #ffffff !important;
    font-weight: bold;
    font-size: 1.7rem;
}

.jumbotron {
    background-color: #282828;
    color: #e0e0e0;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(253, 253, 253, 0.993);
    transition: transform 0.3s ease;
}

.jumbotron:hover {
    transform: translateY(-5px);
}
.intro{
   color: #fdfdfd;
   
   border-radius: 5px;
   /* padding: 80px; */
   /* display: contents; */
  /* display: contents; */
  font-size: 20px;
 
}
img{
   height: 250px;
   width: 250px;
}
.aboutus{
    /* width: 250px;
    height: 350px; */
 transition: 0.5s ease;
 display:flex;
 /* padding: 20px; */
 align-items: center; 


 
}
.aboutus:hover > :not(:hover)
{
    opacity: 0.3;
}
.about:hover{
    transform: scale(1.1);
    box-shadow: 0 8px 16px rgba(105, 1, 109, 0.582);
}
.bird{
    align-items: center;
    display: flex;
    color: #ffffff;
   
   border-radius: 5px;
   /* padding: 80px; */
   /* display: contents; */
  /* display: contents; */
  font-size: 20px;
}
.form-container {
    color: #000000;
    background-color: rgba(214, 214, 214, 0.568); /* Transparent dark */
    padding: 60px;
   width: 600px;
    border-radius: 10px;
    box-shadow: 0 8px 16px rgba(255, 255, 255, 0.897);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    font-style: oblique;
}

.form-container:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 20px rgb(212, 0,200, 255);
}

.form-control {
    background-color: #a5a5a5af;
    color: #ffffff;
    border: 1px solid #ffffff;
    border-radius: 5px;
}

.form-control:focus {
    background-color: #949494;
    border-color: #ec85fa;
    box-shadow: 0 0 5px rgb(0, 0, 0);
    color: rgb(204, 204, 204);
}

.btn-primary {
    background-color: #a08be0;
    border-color: #a08be0;
    transition: background-color 0.3s ease, border-color 0.3s ease;
}

.btn-primary:hover {
    background-color: #8069c0;
    border-color: #8069c0;
}

footer {
    border-top: 1px solid #000000;
    color: #000000;
}

main {
    min-height: calc(100vh - 120px);
    padding: 10px;
}

/* Animations */
.fade-in {
    animation: fadeIn 1s ease-in-out;
}

.slide-in-left {
    animation: slideInLeft 1.7s ease-out;
}
.custom-task-item {
    background-color: #48004e !important; /* or any other color */
    border: 1px solid #dee2e6;
    color: white;

}


@keyframes fadeIn {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}

@keyframes slideInLeft {
    from {
        transform: translateX(-100%);
        opacity: 0;
    }
    to {
        transform: translateX(0);
        opacity: 1;
    }
}
@keyframes gallery{
    0%{transform: rotateY('0deg');}
    100% {transform: rotateY('360deg');}
}
