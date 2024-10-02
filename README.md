# Test
test script login nutacloud
```
import static com.kms.katalon.core.testobject.ObjectRepository.findTestObject
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUI


WebUI.openBrowser('')
WebUI.navigateToUrl('https://nutacloud.com')

WebUI.setText(findTestObject('Object Repository/Page_Login/input_nama_perusahaan'), 'yevs')

WebUI.setText(findTestObject('Object Repository/Page_Login/input_username'), 'Aishy Ash-Shidiq')

WebUI.setEncryptedText(findTestObject('Object Repository/Page_Login/input_password'), 'encrypted_password_here')


WebUI.click(findTestObject('Object Repository/Page_Login/button_login'))

WebUI.verifyElementPresent(findTestObject('Object Repository/Page_Home/element_dashboard'), 10)

WebUI.closeBrowser()
```
