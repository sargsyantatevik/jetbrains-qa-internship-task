# QA Internship Task - Product Analysis (GitHub)

## 1. Selected User Flows

* **Flow 1: Creating and Managing a Repository**
    * **Why:** This is one of the main features of GitHub and is used by most developers, so it is important that the process works correctly.
* **Flow 2: Working with Files and Commits**
    * **Why:** After creating a project, users need to manage content. It is important to verify that files can be added and edited correctly.

---

## 2. Flow 1: Creating and Managing a Repository

### TC-01: Create a Public Repository
**Preconditions:** User is logged in.

**Steps:**
1. Click "+" (top right) → "New repository"
2. Enter repository name (e.g. qa-intern-project)
3. Select "Public"
4. Click "Create repository"

**Expected Result:** Repository is created and opened.

---

### TC-02: Create Repository without Name
**Preconditions:** User is on "Create repository" page.

**Steps:**
1. Leave repository name empty
2. Try to click "Create repository"

**Expected Result:** Creation is not allowed.

---

### TC-03: Create Repository with README
**Preconditions:** User is on "Create repository" page.

**Steps:**
1. Enter repository name
2. Check "Add a README file"
3. Click "Create repository"

**Expected Result:** Repository is created and README file exists.

---

### TC-04: Delete Repository
**Preconditions:** Repository exists.

**Steps:**
1. Open repository
2. Go to "Settings"
3. Scroll to "Danger Zone"
4. Click "Delete this repository"
5. Confirm deletion

**Expected Result:** Repository is removed.

---

### TC-05: Create Repository with .gitignore
**Preconditions:** User is on "Create repository" page.

**Steps:**
1. Enter repository name
2. Check "Add .gitignore"
3. Select template
4. Click "Create repository"

**Expected Result:** Repository is created with .gitignore file.

---

### TC-06: Add Description
**Preconditions:** User is on "Create repository" page.

**Steps:**
1. Enter repository name
2. Add description (e.g. "My first QA project description")
3. Click "Create repository"

**Expected Result:** Description is shown in repository.

---

### TC-07: Rename Repository
**Preconditions:** Repository exists.

**Steps:**
1. Open "Settings"
2. Change repository name (e.g. "renamed-intern-repo")
3. Click "Rename"

**Expected Result:** Repository name is updated.

---

### TC-08: Create Repository with License
**Preconditions:** User is on "Create repository" page.

**Steps:**
1. Enter repository name
2. Select "Add license"
3. Choose MIT license
4. Click "Create repository"

**Expected Result:** Repository is created with LICENSE file.

---

## 3. Flow 2: Working with Files and Commits

### TC-09: Create a New File via Web Interface
**Preconditions:** User is in a repository.

**Steps:**
1. Click "Add file" → "Create new file"
2. Type file name (e.g. manual-test.txt)
3. Write something in the editor
4. Click "Commit changes..."
5. Click "Commit changes"

**Expected Result:** File appears in the repository.

---

### TC-10: Upload a File
**Preconditions:** User is in a repository.

**Steps:**
1. Click "Add file" → "Upload files"
2. Upload a file from computer
3. Wait until upload finishes
4. Click "Commit changes"

**Expected Result:** File appears in the repository.

---

### TC-11: Edit a File
**Preconditions:** File exists.

**Steps:**
1. Open the file
2. Click pencil icon ("Edit this file")
3. Change content
4. Click "Commit changes..."

**Expected Result:** File is updated and new commit is added.

---

### TC-12: Delete a File
**Preconditions:** File exists.

**Steps:**
1. Open the file
2. Click "..."
3. Choose "Delete file"
4. Click "Commit changes"

**Expected Result:** File is removed from repository.

---

### TC-13: Markdown Preview
**Preconditions:** User edits .md file.

**Steps:**
1. Write markdown text (e.g. ## Subtitle)
2. Switch to "Preview"

**Expected Result:** Preview is shown correctly.

---

### TC-14: Commit Without Message
**Preconditions:** User is editing a file.

**Steps:**
1. Make changes
2. Click "Commit changes..."
3. Remove commit message
4. Try to commit

**Expected Result:** Commit is not allowed or a default message is automatically provided.

---

### TC-15: File History
**Preconditions:** File has commits.

**Steps:**
1. Open file
2. Click "History"

**Expected Result:** Commit history is shown chronologically.

---

### TC-16: Copy File Path
**Preconditions:** User is viewing a file.

**Steps:**
1. Click copy icon (Copy path) next to file path
2. Path is copied

**Expected Result:** Path is copied and "Copied!" confirmation appears.
