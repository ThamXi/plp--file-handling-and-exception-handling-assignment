def file_read_write():
    try:
        # Ask user for filename
        filename = input("Enter the filename to read: ")

        # Open and read the original file
        with open(filename, "r") as file:
            content = file.read()

        # Modify content (example: convert to uppercase)
        modified_content = content.upper()

        # Write to a new file
        new_filename = "modified_" + filename
        with open(new_filename, "w") as new_file:
            new_file.write(modified_content)

        print(f"✅ File processed successfully! Modified file saved as '{new_filename}'")

    except FileNotFoundError:
        print("❌ Error: The file does not exist. Please check the filename.")
    except PermissionError:
        print("❌ Error: You do not have permission to read/write this file.")
    except Exception as e:
        print(f"⚠️ Unexpected error: {e}")


# Run the program
if __name__ == "__main__":
    file_read_write()
