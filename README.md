# Spring Boot Folder Structure Generator

This repository contains two scripts that help you generate a pre-defined folder structure for a Spring Boot REST API project. The scripts are available in both Bash (`.sh`) for Linux/MacOS and Batch (`.bat`) for Windows.

## Folder Structure

The scripts will generate the following Spring Boot folder structure:

```
com.example.projectname
│
├── config                         # Configuration classes
├── controller                     # General controllers (non-API)
├── controller.api                 # API-specific controllers (versioned)
│   └── api/v1
│   └── api/v2
├── dto                            # Data Transfer Objects
├── exception                      # Exception handling
├── model                          # Domain models
├── repository                     # Repository classes
├── service                        # Service layer (business logic)
├── mapper                         # Entity-DTO mappers
├── security                       # Security-related classes
└── util                           # Utility classes
```

## How to Use the Scripts

### Download and Run on Linux or MacOS

1. **Download the Bash script**:
   You can use `curl` or `wget` to download the `.sh` file to your local machine.

   - Using `curl`:
     ```bash
     curl -O https://raw.githubusercontent.com/authoritydmc/helpful-scripts/main/generate-spring-boot-structure.sh
     ```

   - Using `wget`:
     ```bash
     wget https://raw.githubusercontent.com/authoritydmc/helpful-scripts/main/generate-spring-boot-structure.sh
     ```

2. **Give Execute Permission**:
   Before running the script, make sure it has executable permissions.
   
   ```bash
   chmod +x generate-spring-boot-structure.sh
   ```

3. **Run the Script**:
   Run the script to generate the folder structure.

   ```bash
   ./generate-spring-boot-structure.sh
   ```

4. **Follow the prompts**:
   The script will show the current directory path and ask for confirmation to proceed. Type `y` to generate the folder structure or `n` to cancel.

---

### Download and Run on Windows

1. **Download the Batch script**:
   Download the `.bat` script using the following command in the command prompt (cmd) or PowerShell:

   ```batch
   curl -O https://raw.githubusercontent.com/authoritydmc/helpful-scripts/main/generate-spring-boot-structure.bat
   ```

   Or, if you have PowerShell:
   ```powershell
   Invoke-WebRequest -Uri https://raw.githubusercontent.com/authoritydmc/helpful-scripts/main/generate-spring-boot-structure.bat -OutFile generate-spring-boot-structure.bat
   ```

2. **Run the Script**:
   Open the command prompt and run the `.bat` script:

   ```batch
   generate-spring-boot-structure.bat
   ```

3. **Follow the prompts**:
   The script will display the current directory and ask if you want to proceed. Type `y` to create the folder structure or `n` to cancel.

---

### Notes:
- Make sure to run the script in the **root directory** of your project or wherever you want to generate the folder structure.
- The folder structure will be created in the **current working directory** where the script is executed.
- These scripts **do not create any files**, they only generate the folder structure for your Spring Boot REST API project.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

