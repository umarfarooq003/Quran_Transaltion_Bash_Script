# Quran Translation Script (QTS)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A Bash script to fetch Quran translations with support for multiple languages and sections (Surah, Ayah, Juz, Ruku).

## Features

- 📖 Fetch translations for specific Surahs, Ayahs, Juz (Para), and Rukus
- 🌍 Support for multiple languages and translators
- 🔍 List available languages and translators
- 🔒 Secure API communication
- 🖥️ Simple command-line interface
- ⚡ Efficient translation retrieval

## Prerequisites

### Required Tools
- **Bash Shell** (default on most Linux/macOS)
- **curl** or **wget**

### Installation Commands
```bash
# Debian-based systems (Ubuntu, Kali)
sudo apt update && sudo apt install curl wget -y

# Red Hat-based systems (CentOS, Fedora)
sudo yum install curl wget -y

# macOS (using Homebrew)
brew install curl wget

## Installation
1. Clone The Repository
```
https://github.com/umarfarooq003/Quran_Transaltion_Bash_Script
cd Quran_Transaltion_Bash_Script
```
2. Make the Script executable
```
chmod +x qts.sh
```
## Usage
```
./qts.sh [options]
```
## Options
```
Option	Description
-h	    Show help message
-l	    List available languages
-L      <lang_code>	List translators for specified language
-e      <lang_code>	Set translation language (default: en)
-t      <translator_code>	Choose specific translator
-s      <surah>	Fetch entire Surah (1-114)
-S      <surah>	Specify Surah for Ayah selection
-A      <ayah>	Fetch specific Ayah from selected Surah
-j      <juz>	Fetch Juz/Para (1-30)
-r      <ruku>	Fetch Ruku (1-40)

```
## Examples
Get entire Surah translation
```
./qts.sh -s 1 -e ar  # Surah Al-Fatihah in Arabic
```
Get specific Ayah
```
./qts.sh -S 2 -A 255 -e en  # Ayatul Kursi in English
```
Get Juz translation
```
./qts.sh -j 1
```
List available languages:
```
./qts.sh -l
```
List Arabic translators:
```
./qts.sh -L ar
```
## How It Works
The script communicates with Quran translation APIs to retrieve requested content. It handles:

Language/translator selection

Parameter validation

API requests formatting

Response parsing and display

## Acknowledgments
Mentors and teachers for guidance

Development team for collaboration

Open source community for support

