# Yarn Cheat Sheet 📌

## 📌 What is Yarn?
Yarn is a fast, reliable, and secure **package manager** for JavaScript projects. It is an alternative to `npm` and offers better performance and stability.

---

## 🛠 Installation Guide
### ✅ Install Yarn (Global Installation)
#### **For Windows (via npm)**
```bash
npm install -g yarn
```
#### **For Mac/Linux (via script)**
```bash
curl -o- -L https://yarnpkg.com/install.sh | bash
```
#### **Check Installed Version**
```bash
yarn --version
```

---

## 🚀 Basic Yarn Commands

### 🔹 Initialize a New Project
```bash
yarn init -y
```
(Generates `package.json` file)

### 🔹 Install All Dependencies
```bash
yarn install
```

### 🔹 Add a New Package
```bash
yarn add package-name
```
Example:
```bash
yarn add react
```

### 🔹 Add a Package as a Dev Dependency
```bash
yarn add package-name --dev
```
Example:
```bash
yarn add eslint --dev
```

### 🔹 Remove a Package
```bash
yarn remove package-name
```
Example:
```bash
yarn remove react
```

### 🔹 Upgrade a Package
```bash
yarn upgrade package-name
```
Example:
```bash
yarn upgrade react
```

### 🔹 Upgrade All Dependencies
```bash
yarn upgrade
```

### 🔹 Clean Cache
```bash
yarn cache clean
```

---

## 🌍 Global Package Management
### 🔹 Install a Global Package
```bash
yarn global add package-name
```
Example:
```bash
yarn global add nodemon
```

### 🔹 Remove a Global Package
```bash
yarn global remove package-name
```
Example:
```bash
yarn global remove nodemon
```

---

## ⚡ Advanced Features
### 🔹 Check Dependency Versions
```bash
yarn list
```

### 🔹 View a Specific Package Version
```bash
yarn info package-name
```

### 🔹 Generate Yarn.lock File
```bash
yarn install --check-files
```

### 🔹 Use Workspaces (For Monorepos)
```json
{
  "workspaces": [
    "packages/*"
  ]
}
```

### 🔹 Enable Plug’n’Play (Faster Installations)
```bash
yarn config set nodeLinker pnp
```

---

## ⚠️ Avoid Mixing `npm` and `yarn` 🚨
**Incorrect Approach:** ❌
```bash
npm install
yarn add react
```
This may cause dependency conflicts.

**Correct Approach:** ✅
Use **only Yarn** or **only npm** for a project.

---

## 🎯 Conclusion
✅ **Yarn is Faster** 🚀  
✅ **Better Dependency Management** 🔥  
✅ **Stable & Secure** 🔒  

Use **Yarn** for improved performance and stability in your JavaScript projects! 🎉
