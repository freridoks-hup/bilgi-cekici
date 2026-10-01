# IOC Extractor

A lightweight Python tool for extracting common Indicators of Compromise (IOCs) from text-based files.

## Features

* Extract IPv4 addresses
* Extract URLs
* Extract email addresses
* Extract domain names
* Detect common hash formats
* Remove duplicate results
* Display a simple summary

## Requirements

* Python 3.x
* No external dependencies

## Usage

```bash
python ioc.py sample.txt
```

The tool reads the provided file and extracts detected indicators.

## Example

Input:

```text
Failed connection from 10.10.10.5
User admin@example.com accessed https://example.org/login
Hash: 5d41402abc4b2a76b9719d911017c592
Another address: 192.168.1.20
```

Çıktı: 

```text
[IP]
  10.10.10.5
  192.168.1.20

[URL]
  https://example.org/login

[EMAIL]
  admin@example.com

[DOMAIN]
  example.org

[HASH]
  5d41402abc4b2a76b9719d911017c592
```

## Proje Durumu 

Bu, Python, düzenli ifadeler, dosya işleme ve temel güvenlik analizi konularına odaklanan bir öğrenme projesidir. 

Proje, ilave IOC türleri, geliştirilmiş ayrıştırma, JSON çıktısı ve daha iyi doğrulama ile genişletilebilir. 

## Yasal Uyarı 

Bu araç, eğitim ve savunma amaçlı güvenlik analizi için tasarlanmıştır. Yalnızca erişim yetkiniz olan dosya ve sistemleri analiz edin.
