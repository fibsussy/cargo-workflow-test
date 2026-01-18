## 🔧 Installation

### One-Line Install (Arch Linux)

**Precompiled binary (default, fast):**
```bash
curl -fsSL https://raw.githubusercontent.com/fibsussy/cargo-workflow-test/main/install.sh | bash
```

**Or build from source:**
```bash
curl -fsSL https://raw.githubusercontent.com/fibsussy/cargo-workflow-test/main/install.sh | bash -s local
```

**Note:** For security, inspect the install script before running it. View it [here](https://github.com/fibsussy/cargo-workflow-test/blob/main/install.sh).

### Manual Installation

#### Prerequisites

Add yourself to the `input` group:
```bash
sudo usermod -a -G input $USER
# Log out and log back in for changes to take effect
```

#### From Source

```bash
# Clone and build
git clone https://github.com/fibsussy/cargo-workflow-test.git
cd cargo-workflow-test
cargo build --release

# Install
sudo cp target/release/cargo-workflow-test /usr/bin/
```

### Post-Installation Setup

1. **Copy the example config:**
```bash
mkdir -p ~/.config/cargo-workflow-test
cp /usr/share/doc/cargo-workflow-test/config.example.ron ~/.config/cargo-workflow-test/config.ron
```

2. **Edit your config:**
```bash
$EDITOR ~/.config/cargo-workflow-test/config.ron
```

3. **Select which keyboards to enable:**
```bash
cargo-workflow-test toggle
```
