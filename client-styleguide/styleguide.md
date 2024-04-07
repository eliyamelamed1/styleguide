# React Folder Structure Documentation

#### Root Level Directories

- **components/**: Contains reusable UI elements.

- **hooks/**: Holds custom React hooks for shared logic.

- **utils/**: Stores utility functions for common tasks.

- **Groups**: Parentheses denote logical grouping (e.g., (ui)/) to enhance organization and navigability.

- **Features**: Modular units of functionality, either shared or page-specific, for scalable code.

#### Features
- **Structure**: Each feature is a self-contained unit, facilitating easy reuse and maintenance.

- **Shared vs. Page-Specific**:
  - Shared features are available application-wide.
  - Page-specific features are tailored for individual pages, containing all necessary logic, components, hooks, and utilities for that page.

- **Feature Entry Point**: index.js acts as the central access point for each feature's functionalities.
Ensures consistent, modular integration across the application.
  - Internal Use: Prefer direct file imports within the feature to avoid dependencies issues.
  - External Use: Use index.js for imports outside the feature for a clean and organized interface. 

#### Pages Directory
- Contains individual pages of the application, each potentially housing exclusive features.

- **Exclusive Features**: Features within a page directory are designed to be used exclusively by that page, emphasizing the importance of tailored functionality to enhance page performance and user experience.

#### Developer's Consideration
- Developers should actively evaluate when to organize root directory folders into groups / features as they grow, ensuring modular and maintainable code structures.


#### Group Syntax Rationale
The use of parentheses (`(ui)/`) as a syntax for naming groups within directories is a strategic choice aimed at enhancing the project's organization. This syntax ensures that grouped directories are prominently visible and listed first in the directory list. The immediate visibility of these groups serves a crucial purpose: it makes it easier for developers to recognize, maintain and and access the project.



### Parentheses Groups vs. Features


* Use features when you have a set of components, hooks, and utilities that together deliver a specific piece of functionality. Features are self-contained, can span across multiple directories, and are designed to be either reused throughout the application or specific to a single page.


#### Examples of Groups vs. Features

#### Groups

**Groups** are meant for organizing related files within a directory, like grouping UI components or hooks that serve similar purposes. They focus on improving folder navigation and clarity.



- **Example of a Group: `(ui)/`**
  - **Purpose:** Organize all UI component-related files that are reused across different parts of the application.
  - **Contents:**
    - `button/`: Includes different button components like `PrimaryButton.js`, `IconButton.js`, etc.
    - `forms/`: Contains form-related components such as `TextInput.js`, `SelectBox.js`, and so on.
    - `layout/`: Houses layout components like `Navbar.js`, `Footer.js`, `Sidebar.js`, etc.
  - **Characteristics:** These components are meant for internal use across the application to maintain a clean and navigable codebase, without directly constituting a standalone feature.

#### Features

**Features** represents a set of components, hooks, and utilities that together deliver a specific piece of functionality. Features are self-contained, can span across multiple directories, and are designed to be either reused throughout the application or specific to a single page.



- **Example of a Feature: `profile`**
  - **Purpose:** Manages and displays user profile information, enabling users to view and edit their details.
  - **Contents:**
    - `components/`: Specific components for the UserProfile feature, like `ProfileForm.js`, `AvatarUpload.js`, etc.
    - `hooks/`: Custom hooks for the UserProfile, for example, `useProfileData.js` for fetching and managing profile data.
    - `utils/`: Utility functions specific to the UserProfile feature, such as form field validators.
    - `index.js`: Serves as the entry point, possibly exporting the main `UserProfile.js` component.
  - **Characteristics:** A self-contained module or feature that has everything needed together, allowing for easy maintenance, updates, or reuse.

This approach ensures the project remains organized, scalable, and maintainable by clearly distinguishing between utility and specific functionality.
