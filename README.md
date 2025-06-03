# cybersecurity
## 🛡 VirusTotal URL Malware Scanner

This Python script integrates with the [VirusTotal API](https://developers.virustotal.com/reference) to scan any URL for potential **malware**, **suspicious behavior**, or **phishing activity**.

### 🔍 Features

* Submits a URL to VirusTotal for analysis.
* Retrieves scan results including:

  * Harmless report count
  * Suspicious report count
  * Malicious report count
* Warns the user if the scanned URL is flagged by any security engines.
* Simple CLI-based interaction.

### 🚀 How It Works

1. The user inputs a URL.
2. The script sends this URL to VirusTotal's public scanning API.
3. It waits \~10 seconds to let the scan complete.
4. It fetches the report and prints the verdict.

### ✅ Sample Output

```
🔍 Submitting URL for scan: http://suspicious-site.com
⏳ Waiting for scan results...

✅ Scan Results:
 - Harmless reports: 65
 - Suspicious reports: 1
 - Malicious reports: 3

⚠ Warning: This URL may be unsafe!
```

### ⚙ Requirements

* Python 3.x
* `requests` module (`pip install requests`)
* A [VirusTotal API Key](https://www.virustotal.com/gui/join-us)

### 🔑 Setup

Replace this line with your actual API key:

```python
API_KEY = 'YOUR_API_KEY_HERE'
```

### ▶ How to Run

```bash
python url_scanner.py
```

You’ll be prompted to enter a URL, and the script will take care of the rest.
