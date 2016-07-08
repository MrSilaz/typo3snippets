# TYPO3 Code Snippets 

TYPO3 Code Snippet integration for Microsoft Studio Visual Code.

**Status**:
- 26 Condition Snippets
- 0 Typoscript Snippets  (soon)
- 0 Fluid Snippets (soon)

Just type the letters 't3' to get a list of all available TYPO3 Code Snippets.

# Screenshot
![Autocomplete](https://raw.githubusercontent.com/MrSilaz/typo3snippets/master/images/snippets.png)

# Snippets for Conditions
Trigger | TYPO3 Code 
--- | --- 
t3ConLanguage |  [language = lang1, lang2, ...]
t3ConIP |   [IP = 192.168.0.0, 192.168.0.0]
t3ConHostname |  [hostname = *.example.com, myhost.*.com]
t3ConApplicationContext |  [applicationContext = context1, context2, ...]
t3ConHour | [hour = hour1, > hour2, < hour3, ...]
t3ConMinute | [minute = minute, > minute, < minute, ...]
t3ConYear | [year  = year , > year , < year , ...]
t3ConDayofweek | [dayofweek  = dayofweek , > dayofweek , < dayofweek  , ...]
t3ConDayofyear | [dayofyear = dayofyear , > dayofyear , < dayofyear , ...]
t3ConUsergroup | [usergroup = group1-uid, group2-uid, ...]
t3ConLogin | [loginUser = fe_users-uid, fe_users-uid, ...]
t3ConUserfunc | [userFunc = user_function(argument1, argument2, ...)]
t3ConPage | [page&#124;field = value]
t3ConTreelevel | [treeLevel = levelnumber, levelnumber, ...]
t3ConPidinrootline | [PIDinRootline = pages-uid, pages-uid, ...]
t3ConPidupinrootline | [PIDupinRootline = pages-uid, pages-uid, ...]
t3ConCompatversion | [compatVersion = x.y.z]
t3ConGvarId | [globalVar = TSFE:id = page_uid&#124;page_uid&#124;page_uid]
t3ConGvarPage | [globalVar = TSFE:page&#124;layout = 1]
t3ConGvarGP | [globalVar = GP:print > 0]
t3ConGvarLit | [globalVar = LIT:1 = {$constant_to_turnSomethingOn}]
t3ConGvarconstant | [globalVar = LIT:1 = {$constant_to_turnSomethingOn}]
t3ConGvarBELogin | [globalVar = TSFE:beUserLogin = 1]
t3ConGvarBEuser | [globalVar = BE_USER&#124;user&#124;uid = 13]
t3ConGStringHost | [globalString = IENV:HTTP_HOST = www.typo3.org]
t3ConGStringReferer | [globalString = IENV:IENV:HTTP_REFERER  = /^$/]
t3ConGString | [globalString = TSFE:page&#124;layout = 1]

# Snippets for Fluid
Trigger | TYPO3 Code 
--- | --- 
t3FluidLinkAction |  <f:link.action pageUid='42' action: 'NULL' >Link</f:link.action>
t3FluidLinkActionInline |  {f:link.action(pageUid: 42, action: 'NULL')}
t3FluidLinkEmail |  <f:link.email email='example@example.com' >E-Mail</f:link.email>
t3FluidLinkEmailInline |  {TYPO3 Fluid inline | f:link.email(email: 'foo')}
t3FluidLinkExternal |  <f:link.external  uri='foo'>Link</f:link.external>
t3FluidLinkExternalInline |  {TYPO3 Fluid inline | f:link.external(uri: '42')}
t3FluidLinkPage |  <f:link.page  pageUid='42'>Link</f:link.page>
t3FluidLinkPageInline |  {TYPO3 Fluid inline | f:link.page(pageUid: '42')}
t3FluidLinkTypolink |  <f:link.typolink parameter='42'>LINK</f:link.typolink>
t3FluidLinkTypolinkInline |  {TYPO3 Fluid inline | f:link.typolink(parameter: '42')}


## Donate & Support
[Donate via PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CJTDRV6L4AR6J)


## Source

All snippets have been taken from [TYPO3.org](https://typo3.org/)
Source on [GitHub](https://github.com/MrSilaz/typo3snippets)
Visual Studio Code [Marketplace](https://marketplace.visualstudio.com/items?itemName=ralffreit.typo3snippets) 
        
## License

[GNU](http://www.gnu.org/licenses/gpl-2.0.html)
