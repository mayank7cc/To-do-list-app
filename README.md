To-Do List App 

This repository contains a simple desktop To-Do List application developed using Java and the Java Swing framework. 
The application allows users to add and delete tasks through an intuitive graphical user interface. It is an excellent project for beginners learning GUI development, event handling, and 
list management in Java.

Features

1.Add new tasks to the task list
2.Delete selected tasks
3.Real-time task display using JList and DefaultListModel
4.Input validation with message prompts
5.Clean and user-friendly interface

Technologies Used
Technology : Java (JDK), Java Swing, DefaultListModel and JList amd JOptionPane.
Usage      : Core programming language, GUI framework, Task handling and display and User notifications.

Application Overview

The interface consists of:
A text field for entering tasks
An Add button to insert tasks into the list
A Delete button to remove selected tasks
A scrollable list displaying all tasks

How the Application Works

Adding a Task
When the user types a task in the input field and clicks "Add", the task is appended to the DefaultListModel and immediately displayed in the JList.
If the input field is empty, a message dialog alerts the user to enter a task. 

Deleting a Task
When the "Delete" button is clicked, the task currently selected in the list is removed.
If no task is selected, a message dialog asks the user to select a task first.

Code Highlights

String task = input.getText();
if (!task.isEmpty()) {
    lm.addElement(task);
    input.setText("");
} else {
    JOptionPane.showMessageDialog(this, "Enter a task.");
}

int index = l1.getSelectedIndex();
if (index != -1) {
    lm.remove(index);
} else {
    JOptionPane.showMessageDialog(this, "Select an item first");
}

Future Enhancements

The project can be improved further by adding features such as:
Marking tasks as completed
Storing tasks permanently using file handling or a database
Editing tasks
Theme customization

Contributing
Contributions and suggestions are welcome. If you encounter issues or have ideas for improvements, you may open an issue or submit a pull request.
