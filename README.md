**Project Description: Simple Version Control System (SVCS)**

This project is a lightweight version control system built using Bash scripts. It provides basic functionality for managing projects, tracking file versions, and handling user access in a collaborative environment. The system ensures only one user can edit a file at a time and allows restoring previous versions when necessary.

### Key Features:

1. **Project Initialization**:
   - Creates new projects with metadata directories and logs activities.
   
2. **User Management**:
   - Supports user sign-in/login with password hashing for security.
   - Tracks and verifies user credentials for file access.

3. **File Check-In/Check-Out**:
   - Allows users to lock files for editing (check-in) and release them (check-out) to prevent simultaneous modifications.

4. **Version Control**:
   - Tracks multiple file versions, automatically incrementing version numbers during check-ins.
   - Allows restoration of specific versions when needed.

5. **Logging of Changes**:
   - Logs all project actions, including commits and restores, with timestamps and user details.

### Core Functions:

- **initProjectDir()**: Creates project directories and initializes metadata.
- **userSignIn() / userLogIn()**: Manages user registration and login.
- **checkInFile() / checkOutFile()**: Controls file locking and unlocking for editing.
- **moveToRepository()**: Saves file versions into the repository.
- **restore()**: Restores a file to a specific version from the repository.

This SVCS is ideal for small projects or teams requiring simple version tracking and file management without the complexity of larger systems like Git.
