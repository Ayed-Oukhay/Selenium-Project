from selenium import webdriver
from selenium.webdriver.common.keys import Keys

# Initialize the Chrome driver
driver = webdriver.Chrome()

# Open Google
driver.get("http://www.google.com")

# Take a screenshot
driver.save_screenshot("screenshot1.png")

# Find the search box
search_box = driver.find_element_by_name("q")

# Type in the search term and submit
search_box.send_keys("Selenium")
search_box.send_keys(Keys.RETURN)

# Take a screenshot
driver.save_screenshot("screenshot2.png")

# Verify the results
assert "Selenium" in driver.title

# Close the browser once done
driver.quit()