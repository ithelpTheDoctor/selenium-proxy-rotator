# Selenium proxy-rotator
A python wrapper around selenium that makes web automation anonymous through elite proxy rotation.

## Features
- Supports incognito
- Random MAC address (this modified for windows so no MAC ADDRESS change)
- Random user agent
- Rotating proxy support for IP change
- Browser geolocation rotation (matches IP from proxy)

## How it works
The algorithm changes the MAC address of your computer. It then initializes the random user agent and proxy IP which is scraped from 3 different elite proxy sources. A Selenium webdriver session is then started where you can automate your web scraping or surfing anonymously.

## Usage
On main.py
```python
    #Open url
    open_url(chromedriver, url)
    time.sleep(5)
    #### Add your own code here.

    # Get session
    print('[+] Session ID: ' + chromedriver.session_id)
    print('[+] Deleting all cookies...')
    chromedriver.delete_all_cookies()
    chromedriver.quit()
```



