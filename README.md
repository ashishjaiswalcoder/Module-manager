# 🚀 Advanced Module Manager

Welcome to **Advanced Module Manager**, an interactive Python CLI tool to efficiently manage your `pip` packages in bulk! With this tool, you can count installed modules, bulk install, or uninstall packages easily.

---

## 🔥 Features

- 🔢 **Count Installed Modules**: View both built-in and external packages with counts.
- 📦 **Bulk Install**: Install multiple packages by typing their names in one line.
- 🗑️ **Bulk Uninstall**: Uninstall several modules at once without confirming each one.
- 🎛️ **Interactive Menu**: Navigate options easily through a clean, emoji-rich interface.

---

## 💾 Installation

1. Clone the repo:
   ```bash
   git clone https://github.com/ashishjaiswalcoder/Module-manager.git
   cd Module-manager
   ```

2. Ensure you have Python 3 installed on your system.

3. (Optional) Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

4. (Optional) Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   *(Note: This project uses `pkg_resources` from setuptools, which is included in most Python installations.)*

---

## 🛠️ Usage

Run the manager script and follow the on-screen prompts:
```bash
python manager.py
```

You'll see a menu like:

1️⃣ Show All Modules (Built-in + External)  
2️⃣ Install Multiple Modules  
3️⃣ Uninstall Multiple Modules  
4️⃣ Exit  

- **Show All Modules**: Lists built-in vs. external packages, with totals.
- **Install Multiple Modules**: Type names separated by spaces (e.g., numpy flask pandas).
- **Uninstall Multiple Modules**: Type names separated by spaces to remove without confirmation flags.

---

## 📋 How It Works

- Uses `sys.builtin_module_names` to gather built-in modules.
- Leverages `pkg_resources.working_set` for external distributions.
- Calls `pip` under the hood via `subprocess` to handle installs and uninstalls.

---

## 🤝 Contributing

Contributions and issues are welcome! 🌟

1. Fork this repo.
2. Create a branch:
   ```bash
   git checkout -b feature/YourFeature
   ```
3. Commit changes:
   ```bash
   git commit -m 'Add feature'
   ```
4. Push:
   ```bash
   git push origin feature/YourFeature
   ```
5. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License. See LICENSE for details.
```