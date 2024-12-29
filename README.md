# gammal-downloader

This is a simple script to download all the content from [gammal.tech](https://www.gammal.tech). It uses the public API.

### public Apis

* [all courses](https://new.gammal.tech/api/products_all)
* [course content](https://new.gammal.tech/api/course/c-programming?contents)

## Requirements

You only need to install yt-dlp and then you may integrate it within your script and modify it according to your needs:

```bash
pip install yt-dlp
pip install requests
```

or

```bash
python3 -m pip yt-dlp
python3 -m requests
```
> It is also better to have [FFmpeg](https://ffmpeg.org) installed on your system.

## Usage

download one video
```bash
python3 downloader.py "https://iframe.mediadelivery.net/embed/{video_library_id}/{video_id}" "video_name" "/path"
```

download all the course

```bash 
dart pub get
dart run index.dart
```
<hr />

## Use on Linux

If Dart is not installed on your Linux distribution, follow the steps below to install it.

> [!NOTE]
> You can use python (OneVideoMethod) Installation on linux as normal with python and pip
>

### 1. Ensure System is Updated

Update your system repositories and install required dependencies:

```bash
sudo apt update
sudo apt install apt-transport-https wget -y
```

### 2. Add Dart's Signing Key

Add Dart's Linux signing key from Google's servers:

```bash
wget -qO- https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo gpg --dearmor -o /usr/share/keyrings/dart-archive-keyring.gpg
```

### 3. Add Dart's Repository

Add Dart's official repository to your system:

```bash
echo "deb [signed-by=/usr/share/keyrings/dart-archive-keyring.gpg] https://storage.googleapis.com/download.dartlang.org/linux/debian stable main" | sudo tee /etc/apt/sources.list.d/dart_stable.list > /dev/null
```

### 4. Install Dart

Update your repositories and install Dart:

```bash
sudo apt update
sudo apt install dart -y
```

---

### 5. Verify Installation

After installation, check Dart's version to confirm it is installed correctly:

```bash
dart --version
```

---

### Notes:

The above steps are for Debian-based distributions (e.g., Ubuntu). For other Linux distributions, refer to [the official Dart installation guide](https://dart.dev/get-dart).

You can now use Dart commands without any issues.
