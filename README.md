# Neat Structure CLI

## Overview
**Neat Structure CLI** is a Node.js-based package designed to enforce absolute consistency in project folder structures. This CLI tool helps developers quickly generate a standardized folder layout for their projects, reducing setup time and ensuring best practices. In future phases, this package will include a dynamic API to enhance its functionality.

---

## Features
- **CLI-based folder structure generation**: Quickly scaffold a consistent project structure.
- **Highly customizable**: Configure the folder structure to suit your needs.
- **Error-free setup**: Ensures folder consistency and eliminates manual errors.

---

## Installation
You can install the package globally using npm:

```bash
npm install -g neat-structure-cli
```

Alternatively, add it to your project dependencies:

```bash
npm install neat-structure-cli --save-dev
```

---

## Usage
### CLI Commands

#### Initialize Folder Structure
Run the following command to initialize a folder structure in your project directory:

```bash
neat init
```

This will create a default folder structure based on the predefined template.

#### Custom Folder Structure
Use the `--config` option to provide a custom configuration file for your folder structure:

```bash
neat init --config <path-to-config-file>
```

### Example Folder Structure
The default structure:
```
src/
  components/
  services/
  utils/
public/
  assets/
    images/
    styles/
```

---

## Configuration
You can customize the folder structure by creating a JSON configuration file (e.g., `folder-config.json`).

### Sample Configuration
```json
{
  "baseDir": "src",
  "folders": [
    "components",
    "services",
    "utils",
    "models"
  ],
  "public": {
    "assets": ["images", "styles"]
  }
}
```

Save the configuration file and run:

```bash
neat init --config folder-config.json
```

---

## Development
### Clone the Repository
To start contributing, clone the repository:

```bash
git clone git@github.com:ialirezaesrafili/neat-structure-cli.git
cd neat-structure-cli
```

### Install Dependencies
Install the required dependencies:

```bash
npm install
```

### Run Locally
Test the CLI locally:

```bash
node index.js init
```

---

## Testing
Run the test suite using:

```bash
npm test
```

---

## Publishing the Package

### Step 1: Upload to GitHub
1. Initialize a Git repository:
   ```bash
   git init
   git remote add origin git@github.com:ialirezaesrafili/neat-structure-cli.git
   ```
2. Commit and push your code:
   ```bash
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git push -u origin main
   ```

### Step 2: Publish to NPM
1. Log in to NPM:
   ```bash
   npm login
   ```
2. Publish your package:
   ```bash
   npm publish
   ```

---

## Future Plans
- **Dynamic API Integration**: Build a robust API for real-time folder management.
- **Template Sharing**: Allow users to share and reuse custom templates.
- **Version Control for Configurations**: Track and manage changes to folder structures over time.

---

## Contributing
We welcome contributions! To contribute:
1. Fork the repository.
2. Create a feature branch.
3. Submit a pull request.

---

## Contact
For feedback or support, please contact:
- Email: [alirezaesrafili553@gmail.com](mailto:alirezaesrafili553@gmail.com)
- GitHub: [ialirezaesrafili](https://github.com/ialirezaesrafili)

---

