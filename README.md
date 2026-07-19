<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>To-Do List App</title>
    <link rel="stylesheet" href="todo-styles.css">
</head>
<body>
    <div class="container">
        <div class="todo-wrapper">
            <header>
                <h1>📝 My To-Do List</h1>
                <p class="subtitle">Stay organized and productive</p>
            </header>

            <!-- Input Section -->
            <div class="input-section">
                <div class="input-group">
                    <input 
                        type="text" 
                        id="todoInput" 
                        placeholder="Add a new task..." 
                        class="todo-input"
                    >
                    <button id="addBtn" class="btn-add">Add Task</button>
                </div>
                <div class="filter-buttons">
                    <button class="filter-btn active" data-filter="all">All</button>
                    <button class="filter-btn" data-filter="active">Active</button>
                    <button class="filter-btn" data-filter="completed">Completed</button>
                </div>
            </div>

            <!-- Stats Section -->
            <div class="stats">
                <div class="stat-item">
                    <span class="stat-label">Total:</span>
                    <span class="stat-value" id="totalCount">0</span>
                </div>
                <div class="stat-item">
                    <span class="stat-label">Active:</span>
                    <span class="stat-value" id="activeCount">0</span>
                </div>
                <div class="stat-item">
                    <span class="stat-label">Completed:</span>
                    <span class="stat-value" id="completedCount">0</span>
                </div>
            </div>

            <!-- Todo List -->
            <div class="todo-list" id="todoList">
                <!-- Tasks will be added here -->
            </div>

            <!-- Empty State -->
            <div class="empty-state" id="emptyState">
                <div class="empty-icon">📭</div>
                <p>No tasks yet. Add one to get started!</p>
            </div>

            <!-- Action Buttons -->
            <div class="action-buttons">
                <button id="clearCompletedBtn" class="btn-secondary">Clear Completed</button>
                <button id="clearAllBtn" class="btn-danger">Clear All</button>
            </div>
        </div>
    </div>

    <script src="todo-script.js"></script>
</body>
</html>
