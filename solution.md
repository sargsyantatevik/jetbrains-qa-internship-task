# QA Internship Task - Product Analysis (GitHub)

## 1. Selected User Flows

*   **Flow 1: Creating and Managing a Repository**
    *   **Why:** This is the most important and main feature of GitHub. A developer's work starts with it, and it is important that the setup is  bug-free.
*   **Flow 2: Working with Files and Commits**
    *   **Why:** After creating a project, users need to manage content. Verifying how files are added or edited ensures the integrity of data storage.
---

## 2. Flow 1: Creating and Managing a Repository

### TC-01: Successful Creation of a Public Repository
**Preconditions:** User is logged into GitHub and is on the home dashboard.
**Steps:**
1. Press the "+" icon in the top right corner and select "New repository".
2. Enter a unique name (e.g., "qa-intern-project") in the field "Repository name".
3. Select the "Public" option.
4. Press the button "Create repository".
**Expected Result:** The user is redirected to the main page of the new repository.

### TC-02: Prevent Creation without a Name
**Preconditions:** User is on the "Create a new repository" page.
**Steps:**
1. Leave the "Repository name" field empty.
2. Scroll down to the "Create repository" button.
**Expected Result:** The button is disabled and cannot be pressed.

### TC-03: Create a Repository with a README File
**Preconditions:** User is on the "Create a new repository" page.
**Steps:**
1. Enter a valid repository name.
2. Check the box "Add a README file".
3. Press "Create repository".
**Expected Result:** The repository is created, and a "README.md" file is visible.

### TC-04: Delete a Repository (Negative/Critical Flow)
**Preconditions:** User is on the home page of their existing repository.
**Steps:**
1. Press the "Settings" tab in the top navigation bar.
2. Scroll to the bottom of the page to the "Danger Zone".
3. Press "Delete this repository".
4.Follow the confirmation instructions.
**Expected Result:** The repository is removed, and there is a confirmation message appears on the dashboard.

### TC-05: Create a Repository with a .gitignore File
**Preconditions:** User is on the "Create a new repository" page.
**Steps:**
1. Enter a valid repository name.
2. Check the box "Add a .gitignore file".
3. Select "ActionScript" (or any other) from the template dropdown.
4. Press "Create repository".
**Expected Result:** The repository is created, and a ".gitignore" file is present in the list.

### TC-06: Verify Repository Description is Displayed
**Preconditions:** User is on the "Create a new repository" page.
**Steps:**
1. Enter a repository name.
2. Enter "Test description" in the Description field.
3. Press "Create repository".
**Expected Result:** The description "Test description" is visible under the name on the repository main page.

### TC-07: Change Repository Name in Settings
**Preconditions:** User is on the main page of a repository they just created.
**Steps:**
1. Press the "Settings" tab.
2. In the "Repository name" field, change the name to something else (e.g., "My project").
3. Press the "Rename" button.
**Expected Result:** The repository name in the header changes to the new name.

### TC-08: Create a Repository with a License
**Preconditions:** User is on the "Create a new repository" page.
**Steps:**
1. Enter a valid name.
2. Check the box "Choose a license".
3. Select "MIT License" from the list.
4. Press "Create repository".
**Expected Result:** The repository is created, and a "LICENSE" file is added to the project.
