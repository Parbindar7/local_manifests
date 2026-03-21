## Getting Started

**1. Initialize repo**
```bash
repo init -u https://github.com/LineageOS/android.git -b lineage-23.2 --git-lfs
```

**2. Clone local manifests**
```bash
git clone https://github.com/Parbindar7/local_manifests.git -b lineage-23.2 .repo/local_manifests
```

**3. Sync source**
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

---

## Build

### Setup Environment

1. Run the environment setup script:
```bash
    . build/envsetup.sh
```

### Build Configuration

1. Choose your device configuration:
```bash
    lunch lineage_$device-$buildtype
```

### Compilation

1. Start the compilation process:
```bash
    m bacon -j$(nproc --all)
```

---


Maintained by **[Parbindar7](https://github.com/Parbindar7)**
