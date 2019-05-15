# Get-Authorization-Value-From-API-Keywords

This plugin is useful to get Authorization value from API.

How to Install plugin:

1. Create/Open Katalon project
2. Click on Plugin Store > Search plugin.
3. Search plugin as Get Authorization value From API Custom Keywords.
4. Click on Get Authorization value From API Custom Keywords plugin.
5. Click on Install button.

How to use:
1. On test case file, import com.plugin.keywords.token.accessToken.getAccessTokenFromAPI Keywords then, use this plugin as below example.
2. Click in input row and then add your AuthorizationKey as string and APIResponce as veriable or you can add the code with com.plugin.keywords.token.accessToken.getAccessTokenFromLoginAPI(AuthorizationKey, APIResponce)
3. Click in Output row and add the result.

Example :
APIResponce = WS.sendRequest(findTestObject('Test API')) // Send API
WS.verifyResponseStatusCode(APIResponce, 200) // Check API responce
def AuthorizationValue = CustomKeywords.'com.plugin.keywords.token.accessToken.getAccessTokenFromAPI'('AuthorizationKey', APIResponce) // Get the Authorization Value
println(AuthorizationValue) // print Authorization value like as d529dd401agghjhjh5138e9babd02774
