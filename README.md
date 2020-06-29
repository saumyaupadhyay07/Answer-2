# Answer-2
import java.util.List;
import java.util.concurrent.TimeUnit;

import org.openqa.selenium.By;
import org.openqa.selenium.Keys;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;
import org.openqa.selenium.support.FindBy;
import org.openqa.selenium.support.ui.ExpectedCondition;
import org.openqa.selenium.support.ui.ExpectedConditions;
import org.openqa.selenium.support.ui.WebDriverWait;

import com.google.common.base.Predicate;
import com.thoughtworks.selenium.Wait;
public class phptravels{

public static void main(String[] args) throws InterruptedException {
  
  WebDriver driver=new FirefoxDriver();
driver.navigate().to("https://www.phptravels.net/home");
  
driver.findElement(By.cssSelector("#usernameId")).sendKeys("Username");
driver.findElement(By.cssSelector("#loginFormId > div.grid_16.alpha.g_box > div.grid_16.alpha > table:nth-child(1) > tbody > tr:nth-child(2) > td:nth-child(2) > input")).sendKeys("");
Thread.sleep(10000); 
driver.findElement(By.name("submit")).click();
Thread.sleep(10000); 
driver.findElement(By.name("Flights")).click();
driver.findElement(By.name("Roundtrip")).click();
WebElement webElementS1= driver.findElement(By.id("class"));
Select select = new Select(element);
select.selectByVisibletext("business");

WebElement webElements2= driver.findElement(By.id("jpform:fromStation"));
  
webElements.sendKeys("NAME OF STATION"); 
webElements.sendKeys(Keys.TAB);
  
Thread.sleep(1000);
   
WebElement webElements3= driver.findElement(By.id("jpform:toStation"));
webElements1.sendKeys("NAME OF STATION"); 
webElements1.sendKeys(Keys.TAB);
  
Thread.sleep(1000);
   
driver.findElement(By.id("jpform:journeyDateInputDate")).sendKeys("");  //Enter Date Of DEPARTURE
driver.findElement(By.id("jpform:journeyDateInputDate")).sendKeys("");  //Enter Date Of ARRIVAL
 
Thread.sleep(3000);
Select AdultDropdown = new Select(driver.findElement(By.id("ctl00_mainContent_ddl_Adult")));

AdultDropdown.selectByValue("2");


Select ChildrenDropdown = new Select(driver.findElement(By.id("ctl00_mainContent_ddl_Child")));
ChildrenDropdown.selectByValue("1");


Select InfantDropdown = new Select(driver.findElement(By.id("ctl00_mainContent_ddl_Infant")));
InfantDropdown.selectByValue("1");
  
driver.findElement(By.id("jpform:jpsubmit")).click(); //Clicks on SUBMIT Button Automatically.
  
Thread.sleep(3000);
  

