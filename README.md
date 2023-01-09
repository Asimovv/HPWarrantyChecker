# **HP Warranty Checker** ![GitHub last commit](https://img.shields.io/github/last-commit/Asimovv/HPWarrantyChecker)

This is a simple python script using Selenium Firefox Driver with the 'webdriver_manager' built in so you don't need to manually download it, to check multiple warranty's status from serial numbers list given by you.

## Requirements
1. Install all the requirements from the 'requirements.txt'.

2. Have an txt file named 'serial_numbers.txt' on the same folder with all serial number that you want to check.

3. Check which region of the serial numbers will be checked and change the website in the code:

```python
driver.get('https://support.hp.com/pt-pt/check-warranty#multiple')
```

1. The xlsx file if not created previous the script will create for you.

2. Run the script with IDE of your choice or run on a terminal.

## ✅**Functionalities**

* Checks the warranty status of all serial numbers in the txt and saves them in an excel file by row.

* Does not overwrite the xlsx data if the script is stopped and started.

## 🟥**Limitations**

* The script will only run a block of 20 serial numbers per loop, for example if your txt has 30 serial numbers, the last 10 will not be checked.
  
* If in the middle of txt has a different region serial number the script will fail.
  
* Doesn't save how many serial numbers it has already checked, so if the script is stopped and started again, it will start at the first serial number in the txt.

## 🚧 **Future ideas**
- [ ] Add a tracker in script to knows where was the last serial number checked and start in the last one.
- [ ] Remove the limitation of 20 serial numbers checked per loop.
- [ ] Change the website region more easily without changing the code manually.
- [ ] Have error checkers in the script so it doesn't fail so easily