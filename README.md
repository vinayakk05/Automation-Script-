# Automation-Script-
# For marking online attendance.
from selenium import webdriver
from selenium.webdriver.common.keys import Keys
import time
import pyautogui

# It will open website
driver=webdriver.Chrome(executable_path="chromedriver.exe");
driver.get("https://weconnect.punecityconnect.org/#/starter/login");

# It will Enter Username
driver.find_element_by_name("username").send_keys("******");
time.sleep(4)

# It will Enter Password
driver.find_element_by_name("password").send_keys("******");

# It will click On Login Button
driver.find_element_by_xpath("//*[@id='mainContent']/div/div/div/app-login/div/div/div/div/div[2]/div/form/div[3]/button/span").click();

# It will Click On Attendance Management Option
time.sleep(4)
driver.find_element_by_link_text("Attendance Management").click();

# It will Click on Student Attendance option
time.sleep(4)
driver.find_element_by_xpath("//*[@id='nav']/app-menu/div[2]/p-panelmenu/div/div[3]/div[2]/div/p-panelmenusub/ul/li[1]/a").click();

# It will Enter Details
time.sleep(8)
driver.find_element_by_xpath("//*[@id='program_id']").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='program_id']/option[2]").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='centre_id']").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='centre_id']/option[2]").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='course_id']").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='course_id']/option[2]").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='batch_id']").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='batch_id']/option[2]").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='attendance_date']/span/input").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='attendance_date']/span/div/div/div[1]/a[1]/span").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='attendance_date']/span/div/div/div[2]/table/tbody/tr[4]/td[7]/a").click();

# It will scroll down web Page
time.sleep(6)
ele=driver.find_element_by_tag_name("html");
ele.send_keys(Keys.END)

time.sleep(4)


time.sleep(4)
driver.find_element_by_xpath("//*[@id='is_present'][1]").click();

time.sleep(4)
driver.find_element_by_xpath("//*[@id='is_present'][1]/option[2]").click();


#driver.find_element_by_xpath("//*[@id='is_present']").click();

#time.sleep(4)
#driver.find_element_by_xpath("//*[@id='is_present']/option[2]").click();

# It is used to click on screen
time.sleep(4)
pyautogui.click(769,396);
pyautogui.click(769,396);
time.sleep(4)
pyautogui.click(769,438);
pyautogui.click(769,438);
pyautogui.click(769,478);
pyautogui.click(769,478);
time.sleep(4)
pyautogui.click(769,518);
pyautogui.click(769,518);
time.sleep(4)
pyautogui.click(769,558);
time.sleep(4)

# Marking Attendance On Next Page
driver.find_element_by_xpath("//*[@id='mainContent']/div/div[2]/div/app-student-attendance-tracking/div/form/div[5]/p-table/div/p-paginator/div/span/a[2]").click();
pyautogui.click(748,356);
pyautogui.click(748,396);
pyautogui.click(748,396);
time.sleep(4)
pyautogui.click(748,438);
pyautogui.click(748,438);
pyautogui.click(748,478);
pyautogui.click(748,478);
time.sleep(4)
pyautogui.click(748,518);
pyautogui.click(748,518);
time.sleep(4)
pyautogui.click(748,558);
time.sleep(4)









