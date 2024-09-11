# Simple To-Do List Application

# Empty list to store tasks
todo_list = []

# Function to display the menu
def show_menu():
    print("\n=== To-Do List Menu ===")
    print("1. View To-Do List")
    print("2. Add a Task")
    print("3. Update a Task")
    print("4. Delete a Task")
    print("5. Exit")

# Function to view tasks in the to-do list
def view_todo_list():
    if len(todo_list) == 0:
        print("\nYour to-do list is empty!")
    else:
        print("\nYour To-Do List:")
        for i, task in enumerate(todo_list, start=1):
            print(f"{i}. {task}")

# Function to add a new task
def add_task():
    task = input("\nEnter the task you want to add: ")
    todo_list.append(task)
    print(f"'{task}' has been added to your to-do list.")

# Function to update an existing task
def update_task():
    view_todo_list()
    if len(todo_list) == 0:
        return
    task_number = int(input("\nEnter the task number you want to update: "))
    if 1 <= task_number <= len(todo_list):
        new_task = input("Enter the new task: ")
        todo_list[task_number - 1] = new_task
        print("Task updated successfully!")
    else:
        print("Invalid task number!")

# Function to delete a task
def delete_task():
    view_todo_list()
    if len(todo_list) == 0:
        return
    task_number = int(input("\nEnter the task number you want to delete: "))
    if 1 <= task_number <= len(todo_list):
        deleted_task = todo_list.pop(task_number - 1)
        print(f"'{deleted_task}' has been deleted from your to-do list.")
    else:
        print("Invalid task number!")

# Main function to run the application
def main():
    while True:
        show_menu()
        choice = input("\nEnter your choice (1-5): ")

        if choice == "1":
            view_todo_list()
        elif choice == "2":
            add_task()
        elif choice == "3":
            update_task()
        elif choice == "4":
            delete_task()
        elif choice == "5":
            print("Exiting the To-Do List Application. Goodbye!")
            break
        else:
            print("Invalid choice! Please enter a number between 1 and 5.")

# Run the main function
if __name__ == "__main__":
    main()
