# TYPO3 Code Snippets 

TYPO3 Code Snippet integration for Microsoft Visual Studio Code.


[![Latest Release](https://vsmarketplacebadge.apphb.com/version-short/ralffreit.typo3snippets.svg)](https://marketplace.visualstudio.com/items?itemName=ralffreit.typo3snippets) 
[![Installs](https://vsmarketplacebadge.apphb.com/installs/ralffreit.typo3snippets.svg)](https://marketplace.visualstudio.com/items?itemName=ralffreit.typo3snippets) 
[![Downloads](https://vsmarketplacebadge.apphb.com/downloads/ralffreit.typo3snippets.svg)](https://marketplace.visualstudio.com/items?itemName=ralffreit.typo3snippets) 
[![Rating](https://vsmarketplacebadge.apphb.com/rating-star/ralffreit.typo3snippets.svg)](https://marketplace.visualstudio.com/items?itemName=ralffreit.typo3snippets&ssr=false#review-details) 


**Current status**:
- 27 Condition Snippets (TYPO3 <= 8)
- 34 Condition Snippets (TYPO3 >= 9)  *NEW*
- 92 Fluid Snippets  (TYPO3 <= 8)
- 79 Fluid Snippets  (TYPO3 >= 9)  *NEW*

Just type the letters 't3' to get a list of all available TYPO3 Code Snippets.

# TYPO3Snippets need your help!
We need more useful high quality snippets visit and open a issue on [//github.com/MrSilaz/typo3snippets/issues](https://github.com/MrSilaz/typo3snippets/issues)

# Screenshot
![Autocomplete](https://raw.githubusercontent.com/MrSilaz/typo3snippets/master/images/snippets.png)


# Snippets for Conditions (>= TYPO3 9.x) *NEW*
Trigger | TYPO3 Code 
--- | --- 
t3ApplicationContext | [applicationContext == "Development"]
t3Page | [page["uid"] == 2]
t3Constant | [{$foo.bar} == 4711]
t3ConstantString | ["{$foo.bar}" == "4711"]
t3Treelevel | [tree.level == 0]
t3TreeRootLineIds | [2 in tree.rootLineIds]
t3TreeRootLine | [tree.rootLine[0]["uid"] == 1]
t3BackendUserIsAdmin | [backend.user.isAdmin]
t3BackendUserIsLoggedIn | [backend.user.isLoggedIn]
t3BackendUserId | [backend.user.userId == 5]
t3BackendUserGroupList | [like(","~backend.user.userGroupList~",", "*,1,*")]
t3FrontendUserIsLoggedIn | [frontend.user.isLoggedIn]
t3FrontendUserId | [frontend.user.userId == 5]
t3FrontendUserGroupList | [like(","~frontend.user.userGroupList~",", "*,1,*")]
t3Typo3Version | [typo3.version == "9.5.5"]
t3Typo3Branch | [typo3.branch == "9.5"]
t3Typo3DevIpMask | [typo3.devIpMask == "172.18.0.6"]
t3RequestGetQueryParams | [request.getQueryParams()['skipSessionUpdate'] == 1]
t3RequestGetParsedBody | [request.getParsedBody()['foo'] == 1]
t3RequestGetHeaders | [request.getHeaders()['Accept'] == 'json']
t3RequestGetCookieParams | [request.getCookieParams()['foo'] == 1]
t3RequestGetNormalizedParams | [request.getNormalizedParams().isHttps()]
t3Date | [date("w") == 7]
t3Like | [like("fooBarBaz", "/f[o]{2,2}[aBrz]+/")]
t3Ip | [ip("172.18.*")]
t3CompatVersion | [compatVersion("9.5")]
t3GetTSFE | [getTSFE().type == 98]
t3Getenv | [getenv("VIRTUAL_HOST") == "docs.typo3.org"]
t3Feature | [feature("TypoScript.strictSyntax") === false]
t3Usergroup | [usergroup("12")]
t3Session | [session("foo|bar") == 1234567]
t3Site | [site("base").getHost() == "docs.typo3.org"]
t3SiteLanguage | [siteLanguage("locale") == "de_CH"]


# Snippets for Conditions (<= TYPO3 8.x)
Trigger | TYPO3 Code 
--- | --- 
t3OldConLanguage |  [language = lang1, lang2, ...]
t3OldConIP |   [IP = 192.168.0.0, 192.168.0.0]
t3OldConHostname |  [hostname = *.example.com, myhost.*.com]
t3OldConApplicationContext |  [applicationContext = context1, context2, ...]
t3OldConHour | [hour = hour1, > hour2, < hour3, ...]
t3OldConMinute | [minute = minute, > minute, < minute, ...]
t3OldConYear | [year  = year , > year , < year , ...]
t3OldConDayofweek | [dayofweek  = dayofweek , > dayofweek , < dayofweek  , ...]
t3OldConDayofyear | [dayofyear = dayofyear , > dayofyear , < dayofyear , ...]
t3OldConUsergroup | [usergroup = group1-uid, group2-uid, ...]
t3OldConLogin | [loginUser = fe_users-uid, fe_users-uid, ...]
t3OldConUserfunc | [userFunc = user_function(argument1, argument2, ...)]
t3OldConPage | [page&#124;field = value]
t3OldConTreelevel | [treeLevel = levelnumber, levelnumber, ...]
t3OldConPidinrootline | [PIDinRootline = pages-uid, pages-uid, ...]
t3OldConPidupinrootline | [PIDupinRootline = pages-uid, pages-uid, ...]
t3OldConCompatversion | [compatVersion = x.y.z]
t3OldConGvarId | [globalVar = TSFE:id = page_uid&#124;page_uid&#124;page_uid]
t3OldConGvarPage | [globalVar = TSFE:page&#124;layout = 1]
t3OldConGvarGP | [globalVar = GP:print > 0]
t3OldConGvarLit | [globalVar = LIT:1 = {$constant_to_turnSomethingOn}]
t3OldConGvarconstant | [globalVar = LIT:1 = {$constant_to_turnSomethingOn}]
t3OldConGvarBELogin | [globalVar = TSFE:beUserLogin = 1]
t3OldConGvarBEuser | [globalVar = BE_USER&#124;user&#124;uid = 13]
t3OldConGStringHost | [globalString = IENV:HTTP_HOST = www.typo3.org]
t3OldConGStringReferer | [globalString = IENV:IENV:HTTP_REFERER  = /^$/]
t3OldConGString | [globalString = TSFE:page&#124;layout = 1]


# Snippets for Fluid (>= TYPO3 9.x) *NEW*
Trigger | TYPO3 Code 
--- | --- 
t3FluidForm | &lt;f:form action=&quot;...&quot; controller=&quot;...&quot; package=&quot;...&quot; enctype=&quot;multipart/form-data&quot;&gt;YourFieldsHere!&lt;/f:form&gt;
t3FluidFormSelect | &lt;f:form.select name=&quot;propertyName&quot; options=&quot;{ObjectOrArray}&quot; optionValueField=&quot;uid&quot; optionLabelField=&quot;firstName&quot; prependOptionLabel=&quot; &quot;/&gt;
t3FluidFormButtonSubmit | &lt;f:form.button&gt;Submit&lt;/f:form.button&gt;
t3FluidFormButtonReset | &lt;f:form.button type=&quot;reset&quot;&gt;Reset&lt;/f:form.button&gt;
t3FluidFormCheckbox | &lt;f:form.checkbox name=&quot;myCheckBox&quot; value=&quot;someValue&quot; /&gt;
t3FluidFormRadio | &lt;f:form.radio name=&quot;myRadioButton&quot; value=&quot;someValue&quot; /&gt;
t3FluidFormHidden | &lt;f:form.hidden name=&quot;myHiddenValue&quot; value=&quot;42&quot; /&gt;
t3FluidFormPassword | &lt;f:form.password name=&quot;myPassword&quot; /&gt;
t3FluidFormSubmit | &lt;f:form.submit value=&quot;Send Mail&quot; /&gt;
t3FluidFormTextarea | &lt;f:form.textarea name=&quot;myTextArea&quot; value=&quot;This is shown inside the textarea&quot; /&gt;
t3FluidFormTextfield | &lt;f:form.textfield name=&quot;myTextBox&quot; value=&quot;default value&quot; /&gt;
t3FluidFormUpload | &lt;f:form.upload name=&quot;file&quot; /&gt;
t3FluidFormValidationResults | &lt;f:if condition=&quot;{validationResults.flattenedErrors}&quot;&gt;<br>&nbsp;&nbsp;&lt;ul class=&quot;errors&quot;&gt;<br>&nbsp;&nbsp;&nbsp;&nbsp;&lt;f:for each=&quot;{validationResults.flattenedErrors}&quot; as=&quot;errors&quot; key=&quot;propertyPath&quot;&gt;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;li&gt;{propertyPath}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;ul&gt;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;f:for each=&quot;{errors}&quot; as=&quot;error&quot;&gt;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;li&gt;{error.code}: {error}&lt;/li&gt;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;/f:for&gt;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;/ul&gt;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;/li&gt;<br>&nbsp;&nbsp;&nbsp;&nbsp;&lt;/f:for&gt;<br>&nbsp;&nbsp;&lt;/ul&gt;<br>&lt;/f:if&gt;<br>&lt;/f:form.validationResults&gt;
t3FluidFormatBytes | &lt;f:format.bytes value=&quot;{fileSize}&quot; decimals=&quot;2&quot; decimalSeparator=&quot;.&quot; thousandsSeparator=&quot;,&quot; /&gt;
t3FluidFormatBytesInline | {fileSize -&gt; f:format.bytes(decimals: 2, decimalSeparator: '.', thousandsSeparator: ',')}
t3FluidFormatCase | &lt;f:format.case mode=&quot;capital&quot; &gt;Some Text with miXed case&lt;/f:format.case&gt;
t3FluidFormatCaseInline | {longtextAsVariable -&gt; f:format.case(mode: 'capital')}
t3FluidFormatCrop | &lt;f:format.crop maxCharacters=&quot;10&quot; &gt;This is some very long text&lt;/f:format.crop&gt;
t3FluidFormatCropInline | {longtextAsVariable -&gt; f:format.crop(maxCharacters: 10)}
t3FluidFormatCurrency | &lt;f:format.currency decimalSeparator=&quot;.&quot; thousandsSeparator=&quot;,&quot; currencySign=&quot;€&quot;&gt;54321&lt;/f:format.currency&gt;
t3FluidFormatCurrencyInline | {54321 -&gt; f:format.currency(decimalSeparator: ',', thousandsSeparator: ',', currencySign: '€')}
t3FluidFormatDate | &lt;f:format.date  format=&quot;{%d. %B %Y}&quot;&gt;{dateObject}&lt;/f:format.date&gt;
t3FluidFormatDateInline | {dateObject -&gt; f:format.date(format: '{%d. %B %Y}')}
t3FluidFormatHtml | &lt;f:format.html  parseFuncTSPath=&quot;lib.parseFunc_RTE&quot;&gt;foo &lt;b&gt;bar&lt;/b&gt;. Some &lt;/f:format.html&gt;
t3FluidFormatHtmlInline | {someTextObject -&gt; f:format.html(parseFuncTSPath: 'lib.parseFunc_RTE')}
t3FluidFormatHtmlentitiesDecodeInline | {someTextObject -&gt; f:format.htmlentitiesDecode(encoding: 'someTextObject')}
t3FluidFormatHtmlentities | &lt;f:format.htmlentities  encoding=&quot;ISO-8859-1&quot;&gt;{text}&lt;/f:format.htmlentities&gt;
t3FluidFormatHtmlentitiesInline | {someTextObject -&gt; f:format.htmlentities(encoding: 'someTextObject')}
t3FluidFormatJson | &lt;f:format.json&gt;{someArray&lt;/f:format.json&gt;
t3FluidFormatJsonInline | {someArray -&gt; f:format.json()}
t3FluidFormatNl2br | &lt;f:format.nl2br&gt;{text_with_linebreaks&lt;/f:format.nl2br&gt;
t3FluidFormatNl2brInline | {text_with_linebreaks -&gt; f:format.nl2br()}
t3FluidFormatNumber | &lt;f:format.number decimals=&quot;1&quot; decimalSeparator=&quot;,&quot; thousandsSeparator=&quot;.&quot;&gt;423423.234&lt;/f:format.number&gt;
t3FluidFormatNumberInline | {423423.234 -&gt; f:format.number(decimals: '1', decimalSeparator: ',', thousandsSeparator: '.')}
t3FluidFormatPadding | &lt;f:format.padding padLength=&quot;10&quot; padString=&quot;-=&quot;&gt;TYPO3&lt;/f:format.padding&gt;
t3FluidFormatPaddingInline | {textObject -&gt; f:format.padding(padLength: '10', padString: '-=')}
t3FluidFormatStripTags | &lt;f:format.stripTags allowedTags=&quot;&lt;p&gt;&lt;span&gt;&lt;div&gt;&lt;script&gt;&quot;&gt;&lt;strong&gt;awesome&lt;strong&gt;&lt;/f:format.stripTags&gt;
t3FluidFormatStripTagsInline | {textObject -&gt; f:format.stripTags(allowedTags: '&lt;p&gt;&lt;span&gt;&lt;div&gt;&lt;script&gt;')}
t3FluidFormatUrlencode | &lt;f:format.urlencode&gt;http://www.freit.de/?encode[this]=1&lt;/f:format.urlencode&gt;
t3FluidFormatUrlencodeInline | {textObject -&gt; f:format.urlencode()}
t3FluidLinkAction | &lt;f:link.action action=&quot;show&quot;&gt;action link&lt;/f:link.action&gt;
t3FluidLinkActionInline | {f:link.action(action: 'show')}
t3FluidLinkEmail | &lt;f:link.email email=&quot;example@domain.tld&quot;&gt;&lt;!-- tag content - may be ignored! --&gt;&lt;/f:link.email&gt;
t3FluidLinkEmailInline | {f:link.email(email: 'example@domain.tld')}
t3FluidLinkExternal | &lt;f:link.external  uri=&quot;http://www.freit.de&quot; target=&quot;_blank&quot;&gt;external link&lt;/f:link.external&gt;
t3FluidLinkExternalInline | {f:link.external(uri: 'http://www.freit.de', target:'_blank')}
t3FluidLinkPage | &lt;f:link.page  pageUid=&quot;1&quot; additionalParams=&quot;{foo: 'bar'}&quot;&gt;page link&lt;/f:link.page&gt;
t3FluidLinkPageInline | {f:link.page(pageUid: '1', additionalParams:'{foo: 'bar'}')}
t3FluidLinkTypolink | &lt;f:link.typolink  parameter=&quot;{link}&quot;&gt;Linktext&lt;/f:link.typolink&gt;
t3FluidLinkTypolinkInline | {f:link.typolink(parameter: '{link}')}
t3FluidSecurityIfAuthenticated | &lt;f:security.ifAuthenticated&gt;<br>&nbsp;&nbsp;&nbsp;his is being shown whenever a FE user is logged in&lt;/f:security.ifAuthenticated&gt;<br>
t3FluidSecurityIfHasRole | &lt;f:security.ifHasRole role=&quot;Administrator&quot;&gt;<br>&nbsp;&nbsp;&nbsp;This is being shown in case the current FE user belongs to a FE usergroup (aka role) titled &quot;Administrator&quot; (case sensitive)<br>&lt;/f:security.ifHasRole&gt;
t3FluidUriAction | &lt;f:uri.action action=&quot;show&quot; /&gt;
t3FluidUriActionInline | {f:uri.action(action: 'show')}
t3FluidUriEmail | &lt;f:uri.email email=&quot;example@domain.tld&quot; /&gt;
t3FluidUriEmailInline | {f:uri.email(email: 'example@domain.tld')}
t3FluidUriExternal | &lt;f:uri.external  uri=&quot;http://www.freit.de&quot; /&gt;
t3FluidUriExternalInline | {f:uri.external(uri: 'http://www.freit.de')}
t3FluidUriImage | &lt;f:uri.image  image=&quot;{imageObject}&quot; /&gt;
t3FluidUriImageInline | {f:uri.image(image: '{imageObject}')}
t3FluidUriPage | &lt;f:uri.page  pageUid=&quot;1&quot; additionalParams=&quot;{foo: \'bar\'}&quot; /&gt;
t3FluidUriPageInline | {f:uri.page(pageUid: '1', additionalParams:'{foo: 'bar'}')}
t3FluidUriResource | &lt;f:uri.resource  path=&quot;css/stylesheet.css&quot; /&gt;
t3FluidUriResourceInline | {f:uri.resource(path: 'css/stylesheet.css')}
t3FluidUriTypolink | &lt;f:uri.typolink  parameter=&quot;{link}&quot; /&gt;
t3FluidUriTypolinkInline | {f:uri.typolink(parameter: '{link}')}
t3FluidWidgetAutocomplete | &lt;f:widget.autocomplete for=&quot;name&quot; objects=&quot;{posts}&quot; searchProperty=&quot;author&quot;&gt;
t3FluidWidgetLink | &lt;f:widget.link action=&quot;show&quot;&gt;show&lt;/f:widget.link&gt;
t3FluidWidgetPaginate | &lt;f:widget.paginate objects=&quot;{blogs}&quot; as=&quot;paginatedBlogs&quot; configuration=&quot;{'itemsPerPage': 10,'insertAbove': false,'insertBelow': true,'maximumNumberOfLinks': 99}&quot;&gt;<br>&nbsp;&nbsp;&nbsp;use \{paginatedBlogs} as you used \{blogs} before, most certainly inside<br>&nbsp;&nbsp;&nbsp;a &lt;f:for&gt; loop.<br>&lt;/f:widget.paginate&gt;<br>
t3FluidWidgetUri | &lt;f:widget.uri action=&quot;show&quot; /&gt;
t3FluidCObject | &lt;f:cObject typoscriptObjectPath=&quot;lib.customHeader&quot; data=&quot;lib.customHeader}&quot; currentValueKey=&quot;lib.customHeader&quot; /&gt;
t3FluidCObjectInline | {article -&gt; f:cObject(typoscriptObjectPath: 'lib.customHeader')}
t3FluidDebug | &lt;f:debug inline=&quot;1&quot; title=&quot;Debug Information&quot;&gt;{arrayOrObject}&lt;/f:debug&gt;
t3FluidImage | &lt;f:image image=&quot;{imageObject}&quot; /&gt;
t3FluidMedia | &lt;f:media file=&quot;{file}&quot;  additionalConfig=&quot;{loop: '1', autoplay: '1'}&quot; /&gt;
t3FluidRender | &lt;f:render partial=&quot;SomePartial&quot; section=&quot;SomePartial&quot; arguments=&quot;{foo: someVariable}&quot; /&gt;
t3FluidRenderInline | {f:render(section: 'SomeSection', partial: 'SomePartial', arguments: {foo: 'someVariable'}, optional: 1)}
t3FluidTranslate | &lt;f:translate key=&quot;htmlKey&quot; htmlEscape=&quot;false&quot; /&gt;
t3FluidTranslateInline | {f:translate(key: 'htmlKey', htmlEscape: 'false')}



# Snippets for Fluid (<= TYPO3 8.x)
Trigger | TYPO3 Code 
--- | --- 
t3OldFluidLinkAction |  &lt;f:link.action pageUid='42' action: 'NULL' &gt;Link&lt;/f:link.action&gt;
t3OldFluidLinkActionInline |  {f:link.action(pageUid: 42, action: 'NULL')}
t3OldFluidLinkEmail |  &lt;f:link.email email='example@example.com'&gt;E-Mail&lt;/f:link.email&gt;
t3OldFluidLinkEmailInline |  {f:link.email(email: 'foo')}
t3OldFluidLinkExternal |  &lt;f:link.external  uri='foo'&gt;Link&lt;/f:link.external&gt;
t3OldFluidLinkExternalInline |  {f:link.external(uri: '42')}
t3OldFluidLinkPage |  &lt;f:link.page  pageUid='42'&gt;Link&lt;/f:link.page&gt;
t3OldFluidLinkPageInline |  {f:link.page(pageUid: '42')}
t3OldFluidLinkTypolink |  &lt;f:link.typolink parameter='42'&gt;LINK&lt;/f:link.typolink&gt;
t3OldFluidLinkTypolinkInline |  {f:link.typolink(parameter: '42')}
t3OldFluidFor | &lt;f:for each='objects' as='obj' iteration='inter'&gt;Content&lt;/f:for&gt;
t3OldFluidForInline | {f:for(each: {object}, as: 'obj', iteration: 'inter')} 
t3OldFluidAlias | &lt;f:alias map=&quot;{amount: '{addresses-&gt;f:count()}'}&quot;&gt;<br>&lt;p&gt;There are {amount} records in database&lt;/p&gt;<br>&lt;/f:alias&gt;
t3OldFluidAliasInline | {f:alias(map: {amount: '{addresses-&gt;f:count()}'})}
t3OldFluidCobject | &lt;f:cObject typoscriptObjectPath=&quot;lib.typoscriptStuff&quot;   data=&quot;{article}&quot; currentValueKey=&quot;title&quot; /&gt;
t3OldFluidCobjectInline | {f:cObject(typoscriptObjectPath: 'foo', data: [mixed], currentValueKey: 'NULL')}
t3OldFluidComment | &lt;f:comment&gt;Wooohooooo!&lt;/f:comment&gt;
t3OldFluidCommentInline | {f:comment('Woohooo')}
t3OldFluidCount | &lt;f:count&gt;{addresses}&lt;/f:count&gt;
t3OldFluidCountInline | {addresses -&gt; f:count()}
t3OldFluidCycle | &lt;f:cycle values=&quot;{0: 'green', 1: 'red', 2: 'blue'}&quot; as=&quot;color&quot;&gt;<br>{color}<br>&lt;/f: cycle&gt;
t3OldFluidCycleInline | {f:cycle(values: {foo: 'bar'}, as: 'foo')}
t3OldFluidDebug | &lt;f:debug title=&quot;NULL&quot; plainText=&quot;1&quot; inline=&quot;0&quot; &gt;{object}&lt;/f: debug&gt;
t3OldFluidDebugInline | {f:debug(title: '$1', plaintext: 1, inline: 1)}
t3OldFluidFlashmessages | &lt;f:flashMessages class=&quot;flashMessage&quot; /&gt;
t3OldFluidFlashmessagesInline | {f:debug(title: 'NULL', plaintext: 1, inline: 1)}
t3OldFluidGroupfor | &lt;f:groupedFor each=&quot;{employees}&quot; as=&quot;employeesByCity&quot; groupBy=&quot;city&quot; groupKey=&quot;city&quot;&gt;<br>&lt;tr&gt;<br>&lt;th colspan=&quot;2&quot;&gt;{city}&lt;/th&gt;<br>&lt;/tr&gt;<br>&lt;f: foreach=&quot;{employeesByCity}&quot; as=&quot;employee&quot;&gt;&lt;tr&gt;&lt;td&gt;{employee.first_name}&lt;/td&gt;&lt;td&gt;{employee.city}&lt;/td&gt;&lt;/tr&gt;&lt;/f: for&gt;&lt;/f: groupedFor&gt;
t3OldFluidGroupforInline | {f:groupedFor(each: {foo: 'bar'}, as: 'foo', groupBy: 'foo', groupKey: ''groupKey'')}
t3OldFluidIf | &lt;f:if condition=&quot;{data}&quot;&gt;&lt;f: then&gt;Thisisbeingshownincasetheconditionmatches.&lt;/f: then&gt;&lt;f: else&gt;ThisisbeingdisplayedincasetheconditionevaluatestoFALSE.&lt;/f: else&gt;&lt;/f: if&gt;
t3OldFluidIfInline | {f:if(condition: someCondition, then: 'condition is met', else: 'condition is not met')}
t3OldFluidImageFal | &lt;f:image  image=&quot;{file}&quot;  width=&quot;NULL&quot; height=&quot;NULL&quot; minWidth=&quot;NULL&quot; minHeight=&quot;NULL&quot; maxWidth=&quot;NULL&quot; maxHeight=&quot;NULL&quot; treatIdAsReference=&quot;1&quot; /&gt;
t3OldFluidImagePath | &lt;f:image  src=&quot;fileadmin/content/demoimage.jpg&quot;  width=&quot;NULL&quot; height=&quot;NULL&quot; minWidth=&quot;NULL&quot; minHeight=&quot;NULL&quot; maxWidth=&quot;NULL&quot; maxHeight=&quot;NULL&quot; alt=&quot; Demo Bild&quot; title=&quot;Demo Bild&quot; /&gt;
t3OldFluidRender | &lt;f:render section=&quot;NULL&quot; partial=&quot;NULL&quot; arguments=&quot;{foo: 'bar'}&quot; optional=&quot;1&quot; /&gt;
t3OldFluidRenderInline | {f:render(section: 'NULL', partial: 'NULL', arguments: {foo: 'bar'}, optional: 1)}
t3OldFluidSwitch | &lt;f:switch expression=&quot;{person.gender}&quot;&gt;<br>&lt;f:case value=&quot;1&quot;&gt;Hello Mr. {person.lastName}&lt;/f:case&gt;<br>&lt;f:case value=&quot;2&quot;&gt;Hello Mrs. {person.lastName}&lt;/f:case&gt;<br>&lt;f:case value=&quot;3&quot;&gt;Hello Miss {person.lastName}&lt;/f:case&gt;<br>&lt;f:case default=&quot;TRUE&quot;&gt;A person with no specified gender&lt;/f:case&gt;<br>&lt;/f:switch&gt;
t3OldFluidSwitchInline | {f:switch(expression: [mixed])}
t3OldFluidTranslate | &lt;f:translate key=&quot;NULL&quot; id=&quot;NULL&quot; default=&quot;NULL&quot; htmlEscape=&quot;1&quot; arguments=&quot;{foo: 'bar'}&quot; extensionName=&quot;NULL&quot; /&gt;
t3OldFluidTranslateInline | {f:translate(key: 'NULL', id: 'NULL', default: 'NULL', htmlEscape: 1, arguments: {foo: 'bar'}, extensionName: 'NULL')}
t3OldFluidFormatBytes | &lt;f:format.bytes value=&quot;123&quot; decimals=&quot;123&quot; decimalSeparator=&quot;.&quot; thousandsSeparator=&quot;,&quot; /&gt;
t3OldFluidFormatBytesInline | {f:format.bytes(value: 123, decimals: 123, decimalSeparator: ''.'', thousandsSeparator: '','')}
t3OldFluidFormatCdata | &lt;f:format.cdata&gt;{data}&lt;/f:format.cdata&gt;
t3OldFluidFormatCdataInline | {f:format.cdata(value: [mixed])}
t3OldFluidFormatCrop | &lt;f:format.crop maxCharacters=&quot;123&quot; append=&quot;...&quot; respectWordBoundaries=&quot;1&quot; respectHtml=&quot;1&quot;&gt;<br>{data}<br>&lt;/f:format.crop&gt;
t3OldFluidFormatCurrency | &lt;f:format.currency currencySign=&quot;$&quot; decimalSeparator=&quot;.&quot; thousandsSeparator=&quot;,&quot; prependCurrency=&quot;TRUE&quot; separateCurrency=&quot;FALSE&quot; decimals=&quot;2&quot;&gt;br{numbers}<br>&lt;/f:format.currency&gt;
t3OldFluidFormatDate | &lt;f:format.date format=&quot;H:i&quot;&gt;$1&lt;/f:format.date&gt;
t3OldFluidFormatHtml | &lt;f:format.html parseFuncTSPath=&quot;lib.parseFunc_RTE&quot;&gt;<br>{data}<br>&lt;/f:format.html&gt;
t3OldFluidFormatHtmlInline | {data-&gt;f:format.html(parseFuncTSPath: 'lib.parseFunc_RTE')}
t3OldFluidFormatHtmlentitiesdecode | &lt;f:format.htmlentitiesDecode value=&quot;NULL&quot; keepQuotes=&quot;1&quot; encoding=&quot;NULL&quot; /&gt;
t3OldFluidFormatHtmlentitiesdecodeInline | {f:format.htmlentitiesDecode(value: 'NULL', keepQuotes: 1, encoding: 'NULL')}
t3OldFluidFormatHtmlentities | &lt;f:format.htmlentitiesDecode value=&quot;NULL&quot; keepQuotes=&quot;1&quot; encoding=&quot;NULL&quot;  doubleEncode=&quot;1&quot;/&gt;
t3OldFluidFormatHtmlentitiesInline | {f:format.htmlentitiesDecode(value: 'NULL', keepQuotes: 1, encoding: 'NULL', doubleEncode:1)}
t3OldFluidFormatHtmlspecialchars | &lt;f:format.htmlspecialchars keepQuotes=&quot;1&quot; encoding=&quot;NULL&quot; doubleEncode=&quot;1&quot;&gt;<br>   &nbsp;&nbsp;&nbsp;{data}&nbsp;<br>&lt;/f:format.htmlspecialchars&gt;
t3OldFluidFormatHtmlspecialcharsInline | {f:format.htmlspecialchars(value: 'NULL', keepQuotes: 1, encoding: 'NULL', doubleEncode: 1)}
t3OldFluidFormatNl2br | &lt;f:format.nl2br value=&quot;Hello World&quot;&gt;
t3OldFluidFormatNl2brInline | {f:format.nl2br(value: 'Hello World')}
t3OldFluidFormatNumber | &lt;f:format.number decimals=&quot;123&quot; decimalSeparator=&quot;.&quot; thousandsSeparator=&quot;,&quot;&gt;{numbers}&lt;/f:format.number&gt;
t3OldFluidFormatNumberInline | {f:format.number(decimals: 123, decimalSeparator: ''.'', thousandsSeparator: '','')}
t3OldFluidFormatPrintf | &lt;f:format.printf arguments=&quot;{0: 3, 1: 'Kasper'}&quot;&gt;<br>   &nbsp;%2$s is great, TYPO%1$d too. Yes, TYPO%1$d is great and so is %2$s.<br>&lt;/f:format.printf&gt;
t3OldFluidFormatPrintfInline | {someText -&gt; f:format.printf(arguments: {1: 'TYPO3'})}
t3OldFluidFormatRaw | &lt;f:format.raw&gt;{string}&lt;/f:format.raw&gt;
t3OldFluidFormatRawInline | {string -&gt; f:format.raw()}
t3OldFluidFormatStriptags | &lt;f:format.stripTags value=&quot;Hello&lt;br&gt;World&quot; /&gt;
t3OldFluidFormatStriptagsInline | {f:format.stripTags(value: 'Hello&lt;br&gt;World')}
t3OldFluidFormatUrlencode | &lt;f:format.urlencode value=&quot;http://www.freit.de &quot; /&gt;
t3OldFluidFormatUrlencodeInline | {f:format.urlencode(value: 'http://www.freit.de')}
t3OldFluidFormButton | &lt;f:form.button type=&quot;submit&quot; name=&quot;NULL&quot; property=&quot;NULL&quot; &gt;Submit&lt;/f:form.button&gt;
t3OldFluidFormButtonInline | {f:form.button(type: 'submit', name: 'NULL', value: 'Submit', property: 'NULL')}
t3OldFluidFormCheckbox | &lt;f:form.checkbox checked=&quot;1&quot;  name=&quot;NULL&quot; value=&quot;foo&quot; property=&quot;NULL&quot; /&gt;
t3OldFluidFormCheckboxInline | {f:form.checkbox(checked: 1,  name: 'NULL', value: 'foo', property: 'NULL')}
t3OldFluidFormHidden | &lt;f:form.hidden name=&quot;NULL&quot; value=&quot;[mixed]&quot; property=&quot;NULL&quot; /&gt;
t3OldFluidFormHiddenInline | {f:form.hidden(name: 'NULL', value: 'foo', property: 'NULL')}
t3OldFluidFormPassword | &lt;f:form.password name=&quot;NULL&quot; value=&quot;[mixed]&quot; property=&quot;NULL&quot;  /&gt;
t3OldFluidFormPasswordInline | {f:form.password(name: 'NULL', value: [mixed], property: 'NULL')}
t3OldFluidFormRadio | &lt;f:form.radio checked=&quot;1&quot; name=&quot;NULL&quot; value=&quot;foo&quot; property=&quot;NULL&quot; /&gt;
t3OldFluidFormRadioInline | {f:form.radio(checked: 1, name: 'NULL', value: 'foo', property: 'NULL')}
t3OldFluidFormTextarea | &lt;f:form.textarea name=&quot;NULL&quot; property=&quot;NULL&quot; rows=&quot;[anySimpleType]&quot; cols=&quot;[anySimpleType]&quot;&gt;&lt;/f:form.textarea&gt;
t3OldFluidFormTextfield | &lt;f:form.textfield type=&quot;text&quot; name=&quot;NULL&quot; value=&quot;[mixed]&quot; property=&quot;NULL&quot;  /&gt;
t3OldFluidFormTextfieldInline | {f:form.textfield(type: 'text, name: 'NULL', value: [mixed], property: 'NULL')}
t3OldFluidFormUpload | &lt;f:form.upload name=&quot;NULL&quot; property=&quot;NULL&quot; multiple=&quot;NULL&quot; /&gt;
t3OldFluidFormUploadInline | {f:form.upload(name: 'NULL', property: 'NULL', multiple: '1')}
t3OldFluidUriAction | &lt;f:uri.action action=&quot;NULL&quot; pageUid=&quot;123&quot;  /&gt;
t3OldFluidUriActionInline | {f:uri.action(action: 'NULL', pageUid: 123}
t3OldFluidUriEmail | &lt;f:uri.email email=&quot;foo&quot;&gt;
t3OldFluidUriEmailInline | {f:uri.email(email: '$1')}
t3OldFluidUriExternal | &lt;f:uri.external uri=&quot;freit.de&quot; defaultScheme=&quot;http&quot; /&gt;
t3OldFluidUriExternalInline | {f:uri.external(uri: '$1', defaultScheme: 'http')}
t3OldFluidUriImage | &lt;f:uri.image src=&quot;NULL&quot; image=&quot;[anySimpleType]&quot; width=&quot;NULL&quot; height=&quot;NULL&quot; treatIdAsReference=&quot;1&quot; /&gt;
t3OldFluidUriImageInline | {f:uri.image(src: 'NULL', image: [anySimpleType], width: 'NULL', height: 'NULL', treatIdAsReference: 1)}
t3OldFluidUriPage | &lt;f:uri.page pageUid=&quot;42&quot;  /&gt;
t3OldFluidUriPageInline | {f:uri.page(pageUid: 23)}
t3OldFluidUriTypolink | &lt;f:uri.typolink parameter=&quot;foo&quot; additionalParams=&quot;&quot;&gt;
t3OldFluidUriTypolinkInline | {f:uri.typolink(parameter: 'foo', additionalParams: ')}


## Donate & Support
Hello and thank you so much for using this extension. I use a lot of my free time and it takes me a lot of effort to maintain this
FREE feature and to keep it up-to-date.

Of course I do this because I love the work that I do and the possibilities I can provide through it,
but I surely wouldn’t be mad if you or your agency would decide to donate something in return.

I’d be thankful for any sort of amount via PayPal. And even if you’re looking to donate something other than money,
I’d love for you to take a look at my wishlist.
If you’re especially generous you might even get a special place in this readme :-) .

[Donate via PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CJTDRV6L4AR6J)
[Donate via Amazon.de](https://www.amazon.de/hz/wishlist/ls/1YMK0VR1GQXR5)

Thank you :-*


## Source

All snippets have been taken from [TYPO3.org](https://typo3.org/) 
Source on [GitHub](https://github.com/MrSilaz/typo3snippets) 
On Visual Studio [Marketplace](https://marketplace.visualstudio.com/items?itemName=ralffreit.typo3snippets) 


## Helpful links
TYPO3 Fluid ViewHelper Reference [visit](https://docs.typo3.org/other/typo3/view-helper-reference/9.5/en-us/typo3/fluid/latest/Index.html)
TYPO3 Condition Reference [visit](https://docs.typo3.org/m/typo3/reference-typoscript/9.5/en-us/Conditions/#reference)
Convert Fluid tags into inline notation [visit](http://www.fluid-converter.com/)
        
## License
[GNU](http://www.gnu.org/licenses/gpl-2.0.html)

## Changelog
**0.1.0** 
- 34 new Condition Snippets for TYPO3 > 9
- 79 new Fluid Snippets for TYPO3 > 9
- All old Snippets tagged with "old" (e.g. t3Old...)
- Online form http://typo3snippets.freit.de/  (dropped) ([please Use GitHub Issuses](https://github.com/MrSilaz/typo3snippets/issues))


**0.0.9** 
- Super awesome spezial bugfixfix :-D

**0.0.8** 
- Add new Online form to add snippets ( http://typo3snippets.freit.de/ )
- Small bugfixes

**0.0.7** 
- New File Type Association with .ts, .fluid and .t3
- New Language "TypoScript" (! conflict with TypeScript, you need to change your settings manually)
- Fluid and Typoscript add to HTML Language autocomplete


**0.0.6**
- 42 Fluid Snippets addet, little Readme fixes