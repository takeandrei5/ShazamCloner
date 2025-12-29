# ShazamCloner

## How to Add Remote Origin

If you've cloned this repository locally and want to set up a remote origin (or change it to your own repository), follow these steps:

### Adding a Remote Origin

If your local repository doesn't have a remote origin configured yet, you can add one with:

```bash
git remote add origin <your-repository-url>
```

For example:
```bash
git remote add origin https://github.com/yourusername/your-repo.git
```

Or using SSH:
```bash
git remote add origin git@github.com:yourusername/your-repo.git
```

### Changing an Existing Remote Origin

If you want to change the URL of an existing remote origin:

```bash
git remote set-url origin <new-repository-url>
```

For example:
```bash
git remote set-url origin https://github.com/yourusername/your-repo.git
```

### Verifying Your Remote Configuration

To check your current remote configuration:

```bash
git remote -v
```

This will show you the URLs for fetch and push operations.

### Common Git Remote Operations

Once your remote origin is configured, you can:

**Push your changes:**
```bash
git push -u origin main
```

**Pull updates:**
```bash
git pull origin main
```

**Fetch changes without merging:**
```bash
git fetch origin
```

### Removing a Remote

If you need to remove a remote:

```bash
git remote remove origin
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
