# ⚙️ Bios

> Batch script to apply **BCD (Boot Configuration Data)** tweaks that affect low-level boot and virtualization settings.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🔧 **BCD Tweaks** | Modifies boot configuration via `bcdedit` |
| 🛡️ **Security / Performance** | NX, EMS, TPM, ELAM, hypervisor, and related options |
| 📋 **Legacy Boot** | Sets boot menu policy to Legacy |

---

## 📋 Requirements

| Requirement | Details |
|-------------|---------|
| **OS** | Windows 10/11, Server |
| **Privileges** | Administrator |

---

## 🚀 Usage

```cmd
:: Run as Administrator
Bios.cmd
```

---

## 🔧 Tweaks Applied

| Setting | Value |
|---------|-------|
| NX | AlwaysOff |
| EMS / bootems | No |
| Integrity services | disable |
| TPM boot entropy | ForceDisable |
| Boot menu policy | Legacy |
| ELAM drivers | disable |
| Hypervisor launch type | off |
| PAE | ForceDisable |
| X2APIC policy | disable |

---

## ⚠️ Warning

These changes affect boot security and virtualization. Use only if you understand the implications. Create a restore point first.

---

<p align="center">
  <sub>🔧 Gorstak Windows Security Tooling</sub>
</p>
