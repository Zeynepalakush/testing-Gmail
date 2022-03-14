# testing-Gmail
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
 public class testDriverEmail {
       Public static void main(String[] args) {

  // setting driver properties
System.setProperty(“webdriver.chrome.driver”,”/Users/ganeshdhareswar/Downloads/chromedriver”);
WebDriver driver = new ChromeDriver();

//navigate ur driver to mail.google.com
driver.navigate().to(http://mail.google.com);

//enter email id
driver.findElement(By.cssSelector(“#Email”)).sendKeys(“automationfunworlQgmail.com”);

//click on next button
driver.findElement(By.cssSelector(“#next”)).click();
driver.manage().timeouts().implicitlyWait(2,TimeUnit,SECONDS);

//enter pasword
driver.findElement(By.cssSelector(“#password).sendKeys(“automation2016”);

//click sign in button 
driver.findElement(By.cssSelector(“#signIn”)).click();
driver.close();
driver.quit();


   }
}
