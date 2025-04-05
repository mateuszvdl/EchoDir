# EchoDir
Echo your directory into a log file — clean and simple.

## 🚀 Features

- **Write (`w`)** – Save the current list of files (sorted in reverse order) into `listaplikow.txt`, overwriting any previous content.
- **Append (`a`)** – Add the current list of files to the end of `listaplikow.txt`.
- **Read (`r`)** – Display the contents of `listaplikow.txt`.

## 🧠 How It Works

Based on a single input parameter, the script executes different actions:

| Option | Description |
|--------|-------------|
| `w`    | Write current directory file list to `listaplikow.txt` |
| `a`    | Append current directory file list to `listaplikow.txt` |
| `r`    | Read and print the contents of `listaplikow.txt` |
| Other  | Shows an error message with usage info |

## 📝 Usage

```bash
./script.sh [option]
```

Replace `[option]` with one of the following:

- `w` – Write mode
- `a` – Append mode
- `r` – Read mode

### Example

```bash
./script.sh w   # Overwrites the list with current directory contents
./script.sh a   # Appends current directory contents to the list
./script.sh r   # Displays the stored list
```

## 📂 Output File

All file listings are saved in:
```
listaplikow.txt
```

> **Note:** Files are listed in reverse order (newest last), as per the `ls -1r` command.

## ⚠️ Error Handling

- If no parameter or an unknown parameter is provided, the script shows a usage message.
- If reading (`r`) is requested but `listaplikow.txt` does not exist, an error message is shown.

## ✅ Requirements

- Bash shell
- Unix-like system (Linux/macOS)

## 📌 License

This project is open-source. Feel free to modify and use it as needed!
