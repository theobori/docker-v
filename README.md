# 🐋 docker-v

A tiny CLI to import and export Docker volumes.

## 📖 How to build and run ?
1. Install the dependencies
    - `bash>=4.0` (or at least a shell supporting bash)


## ⭐ Use cases

Here are some usage examples.

### 📥 Export

Export a Docker volume to a directory

```bash
./docker-v \
    -v volume_name \
    -e
```

Export a Docker volume to a tarball

```bash
./docker-v \
    -v volume_name \
    -a output.tar.gz \
    -e
```

### 📤 Import

Import a directory to a Docker volume

```bash
./docker-v \
    -v volume_name \
    -d input_dir -i
```

Import a tarball (then extract) to a Docker volume

```bash
./docker-v \
    -v volume_name \
    -d dir_path \
    -a input.tar.gz \
    -i
```

## ℹ️ Scripts informations

To get more informations about the CLI arguments, you can run `./docker-v -h`.