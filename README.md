# NewNellaRead123

Add a new for trainings 

add more details 
package JqueryUiHomework;

import java.time.Duration;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.annotations.Test;


public class Jquery {
	

	private WebDriver driver; // variable driver
	private String websiteURL = "https://jqueryui.com/draggable/";
	@Test
	public void StartJquery()  {
		try {

			// System.setProperty("webdriver.chrome.driver",
						// "src\\test\\resources\\drivers\\chromedriver.exe");
					// start chrome driver 
					System.out.println(" Step1 : opening the chrom driver");
					driver = new ChromeDriver();
					driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(30));
					driver.manage().timeouts().pageLoadTimeout(Duration.ofSeconds(30));
					driver.manage().window().maximize();
					driver.get(websiteURL);   //Get the website title 
					driver.getTitle();
					Thread.sleep(5 * 1000);
