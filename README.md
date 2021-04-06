# Test-project-task
A test project for a task
# Test-project
//pre requisite
//import Selenium webdriver/
/Navigate to the url 
//Click one of the defined links on the page

// This is a Basic Smoke test only high level

Webdriver = new Chromedriver ();
driver.get("http://computer-database.herokuapp.com/computers")

//Click a link on the page
driver.find_element_by_link_text
("Name of link").click()

//Alternatively
//This has a wait after loading the web page and selects the text within the returned web page
import java.util.concurrent.TimeUnit;
 
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
 
public class LinkText {
 
  public static void main(String[] args) {
   
   // TODO Auto-generated method stub
    
    System.setProperty("webdriver.chrome.driver", ".\\ChromeDriver\\chromedriver.exe");
    WebDriver driver=new ChromeDriver();
    driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
    
    driver.manage().window().maximize();
    
    //Opening the ("http://computer-database.herokuapp.com/computers")
    driver.get("http://computer-database.herokuapp.com/computerl");
    
    //locating an element via link text in Selenium now, and clicking on that element name "A test 123" 
    driver.findElement(By.linkText("A test 123")).click();
 
            driver.quit();
  }
 
}
