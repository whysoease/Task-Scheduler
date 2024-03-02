# Task Scheduler

Task Scheduler is a lightweight JavaScript package for scheduling tasks to run after a specified delay.

## Installation

To install Task Scheduler, you can use npm:

```
npm install task-scheduler
```

## Usage

```javascript
const TaskScheduler = require('task-scheduler');

// Initialize Task Scheduler
const scheduler = new TaskScheduler();

// Schedule a task
const task1 = scheduler.scheduleTask(() => {
  console.log('Task 1 executed');
}, 2000);

// Cancel a task
scheduler.cancelTask(task1);

// Clear all tasks
scheduler.clearAllTasks();
```

## API

### `scheduleTask(task, delay)`

Schedules a task to run after the specified delay (in milliseconds).

- `task`: The task to be executed.
- `delay`: The delay (in milliseconds) before the task is executed.

Returns an object representing the scheduled task.

### `cancelTask(taskObj)`

Cancels the specified task.

- `taskObj`: The task object returned by `scheduleTask`.

### `clearAllTasks()`

Clears all scheduled tasks.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
