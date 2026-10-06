# Automation

### Selenium Demo for Automation
```
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import Select
import time

driver = webdriver.Chrome()

driver.get("https://vinothqaacademy.com/demo-site/")
driver.maximize_window()

time.sleep(3)

# Get all input fields belonging to Registration Form
inputs = driver.find_elements(
    By.XPATH,
    "//h3[contains(normalize-space(),'Registration Form')]/following::input"
)


inputs[0].send_keys("Prashanth")

inputs[1].send_keys("K")

inputs[2].click()

inputs[5].click()

inputs[11].send_keys("123 Main Street")

inputs[12].send_keys("A101")


inputs[13].send_keys("Chennai")

inputs[14].send_keys("Tamil Nadu")

inputs[15].send_keys("600001")

inputs[16].send_keys("Prashanth@gmail.com")

inputs[17].send_keys("10/06/26")

inputs[18].send_keys("9840524745")

inputs[20].send_keys("33")

time.sleep(30)
```

### Output:
<img width="1732" height="743" alt="image" src="https://github.com/user-attachments/assets/54179a0d-afcb-4072-8b4f-3ae6892af45b" />

