# task-6c

def write_employee_report(filename):
    """Writes a report of employees to the specified file."""
    employees = [
        {"name": "Alice", "department": "HR"},
        {"name": "Bob", "department": "Engineering"},
        {"name": "Charlie", "department": "Finance"}
    ]

    # Open the file in write mode
    with open(filename, "w") as file:
        for employee in employees:
            # Write the employee data to the file
            line = f"Name: {employee['name']}, Department: {employee['department']}\n"
            file.write(line)

# Example usage:
write_employee_report("employee_report.txt")
