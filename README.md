# TYPO3 Code Snippets 

TYPO3 Code Snippet integration for Microsoft Studio Visual Code.

**Status**:
- 27 Condition Snippets
- 0 Typoscript Snippets  (soon)
- 51 Fluid Snippets (soon more)

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
t3FluidLinkAction |  &lt;f:link.action pageUid='42' action: 'NULL' &gt;Link&lt;/f:link.action&gt;
t3FluidLinkActionInline |  {f:link.action(pageUid: 42, action: 'NULL')}
t3FluidLinkEmail |  &lt;f:link.email email='example@example.com'&gt;E-Mail&lt;/f:link.email&gt;
t3FluidLinkEmailInline |  {f:link.email(email: 'foo')}
t3FluidLinkExternal |  &lt;f:link.external  uri='foo'&gt;Link&lt;/f:link.external&gt;
t3FluidLinkExternalInline |  {f:link.external(uri: '42')}
t3FluidLinkPage |  &lt;f:link.page  pageUid='42'&gt;Link&lt;/f:link.page&gt;
t3FluidLinkPageInline |  {f:link.page(pageUid: '42')}
t3FluidLinkTypolink |  &lt;f:link.typolink parameter='42'&gt;LINK&lt;/f:link.typolink&gt;
t3FluidLinkTypolinkInline |  {f:link.typolink(parameter: '42')}
t3FluidFor | &lt;f:for each='objects' as='obj' iteration='inter'&gt;Content&lt;/f:for&gt;
t3FluidForInline | {f:for(each: {object}, as: 'obj', iteration: 'inter')} 
t3FluidAlias | &lt;f:alias map=&quot;{amount: '{addresses-&gt;f:count()}'}&quot;&gt;<br>&lt;p&gt;There are {amount} records in database&lt;/p&gt;<br>&lt;/f:alias&gt;
t3FluidAliasInline | {f:alias(map: {amount: '{addresses-&gt;f:count()}'})}
t3FluidCobject | &lt;f:cObject typoscriptObjectPath=&quot;lib.typoscriptStuff&quot;   data=&quot;{article}&quot; currentValueKey=&quot;title&quot; /&gt;
t3FluidCobjectInline | {f:cObject(typoscriptObjectPath: 'foo', data: [mixed], currentValueKey: 'NULL')}
t3FluidComment | &lt;f:comment&gt;Wooohooooo!&lt;/f:comment&gt;
t3FluidCommentInline | {f:comment('Woohooo')}
t3FluidCount | &lt;f:count&gt;{addresses}&lt;/f:count&gt;
t3FluidCountInline | {addresses -&gt; f:count()}
t3FluidCycle | &lt;f:cycle values=&quot;{0: 'green', 1: 'red', 2: 'blue'}&quot; as=&quot;color&quot;&gt;<br>{color}<br>&lt;/f: cycle&gt;
t3FluidCycleInline | {f:cycle(values: {foo: 'bar'}, as: 'foo')}
t3FluidDebug | &lt;f:debug title=&quot;NULL&quot; plainText=&quot;1&quot; inline=&quot;0&quot; &gt;{object}&lt;/f: debug&gt;
t3FluidDebugInline | {f:debug(title: '$1', plaintext: 1, inline: 1)}
t3FluidFlashmessages | &lt;f:flashMessages class=&quot;flashMessage&quot; /&gt;
t3FluidFlashmessagesInline | {f:debug(title: 'NULL', plaintext: 1, inline: 1)}
t3FluidGroupfor | &lt;f:groupedFor each=&quot;{employees}&quot; as=&quot;employeesByCity&quot; groupBy=&quot;city&quot; groupKey=&quot;city&quot;&gt;<br>&lt;tr&gt;<br>&lt;th colspan=&quot;2&quot;&gt;{city}&lt;/th&gt;<br>&lt;/tr&gt;<br>&lt;f: foreach=&quot;{employeesByCity}&quot; as=&quot;employee&quot;&gt;&lt;tr&gt;&lt;td&gt;{employee.first_name}&lt;/td&gt;&lt;td&gt;{employee.city}&lt;/td&gt;&lt;/tr&gt;&lt;/f: for&gt;&lt;/f: groupedFor&gt;
t3FluidGroupforInline | {f:groupedFor(each: {foo: 'bar'}, as: 'foo', groupBy: 'foo', groupKey: ''groupKey'')}
t3FluidIf | &lt;f:if condition=&quot;{data}&quot;&gt;&lt;f: then&gt;Thisisbeingshownincasetheconditionmatches.&lt;/f: then&gt;&lt;f: else&gt;ThisisbeingdisplayedincasetheconditionevaluatestoFALSE.&lt;/f: else&gt;&lt;/f: if&gt;
t3FluidIfInline | {f:if(condition: someCondition, then: 'condition is met', else: 'condition is not met')}
t3FluidImageFal | &lt;f:image  image=&quot;{file}&quot;  width=&quot;NULL&quot; height=&quot;NULL&quot; minWidth=&quot;NULL&quot; minHeight=&quot;NULL&quot; maxWidth=&quot;NULL&quot; maxHeight=&quot;NULL&quot; treatIdAsReference=&quot;1&quot; /&gt;
t3FluidImagePath | &lt;f:image  src=&quot;fileadmin/content/demoimage.jpg&quot;  width=&quot;NULL&quot; height=&quot;NULL&quot; minWidth=&quot;NULL&quot; minHeight=&quot;NULL&quot; maxWidth=&quot;NULL&quot; maxHeight=&quot;NULL&quot; alt=&quot; Demo Bild&quot; title=&quot;Demo Bild&quot; /&gt;
t3FluidRender | &lt;f:render section=&quot;NULL&quot; partial=&quot;NULL&quot; arguments=&quot;{foo: 'bar'}&quot; optional=&quot;1&quot; /&gt;
t3FluidRenderInline | {f:render(section: 'NULL', partial: 'NULL', arguments: {foo: 'bar'}, optional: 1)}
t3FluidSwitch | &lt;f:switch expression=&quot;{person.gender}&quot;&gt;<br>&lt;f:case value=&quot;1&quot;&gt;Hello Mr. {person.lastName}&lt;/f:case&gt;<br>&lt;f:case value=&quot;2&quot;&gt;Hello Mrs. {person.lastName}&lt;/f:case&gt;<br>&lt;f:case value=&quot;3&quot;&gt;Hello Miss {person.lastName}&lt;/f:case&gt;<br>&lt;f:case default=&quot;TRUE&quot;&gt;A person with no specified gender&lt;/f:case&gt;<br>&lt;/f:switch&gt;
t3FluidSwitchInline | {f:switch(expression: [mixed])}
t3FluidTranslate | &lt;f:translate key=&quot;NULL&quot; id=&quot;NULL&quot; default=&quot;NULL&quot; htmlEscape=&quot;1&quot; arguments=&quot;{foo: 'bar'}&quot; extensionName=&quot;NULL&quot; /&gt;
t3FluidTranslateInline | {f:translate(key: 'NULL', id: 'NULL', default: 'NULL', htmlEscape: 1, arguments: {foo: 'bar'}, extensionName: 'NULL')}
t3FluidFormatBytes | &lt;f:format.bytes value=&quot;123&quot; decimals=&quot;123&quot; decimalSeparator=&quot;.&quot; thousandsSeparator=&quot;,&quot; /&gt;
t3FluidFormatBytesInline | {f:format.bytes(value: 123, decimals: 123, decimalSeparator: ''.'', thousandsSeparator: '','')}
t3FluidFormatCdata | &lt;f:format.cdata&gt;{data}&lt;/f:format.cdata&gt;
t3FluidFormatCdataInline | {f:format.cdata(value: [mixed])}
t3FluidFormatCrop | &lt;f:format.crop maxCharacters=&quot;123&quot; append=&quot;...&quot; respectWordBoundaries=&quot;1&quot; respectHtml=&quot;1&quot;&gt;<br>{data}<br>&lt;/f:format.crop&gt;
t3FluidFormatCurrency | &lt;f:format.currency currencySign=&quot;$&quot; decimalSeparator=&quot;.&quot; thousandsSeparator=&quot;,&quot; prependCurrency=&quot;TRUE&quot; separateCurrency=&quot;FALSE&quot; decimals=&quot;2&quot;&gt;br{numbers}<br>&lt;/f:format.currency&gt;
t3FluidFormatDate | &lt;f:format.date format=&quot;H:i&quot;&gt;$1&lt;/f:format.date&gt;
t3FluidFormatHtml | &lt;f:format.html parseFuncTSPath=&quot;lib.parseFunc_RTE&quot;&gt;<br>{data}<br>&lt;/f:format.html&gt;
t3FluidFormatHtmlInline | {data-&gt;f:format.html(parseFuncTSPath: 'lib.parseFunc_RTE')}
t3FluidFormatHtmlentitiesdecode | &lt;f:format.htmlentitiesDecode value=&quot;NULL&quot; keepQuotes=&quot;1&quot; encoding=&quot;NULL&quot; /&gt;
t3FluidFormatHtmlentitiesdecodeInline | {f:format.htmlentitiesDecode(value: 'NULL', keepQuotes: 1, encoding: 'NULL')}
t3FluidFormatHtmlentities | &lt;f:format.htmlentitiesDecode value=&quot;NULL&quot; keepQuotes=&quot;1&quot; encoding=&quot;NULL&quot;  doubleEncode=&quot;1&quot;/&gt;
t3FluidFormatHtmlentitiesInline | {f:format.htmlentitiesDecode(value: 'NULL', keepQuotes: 1, encoding: 'NULL', doubleEncode:1)}





## Donate & Support
[Donate via PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CJTDRV6L4AR6J)


## Source

All snippets have been taken from [TYPO3.org](https://typo3.org/)
Source on [GitHub](https://github.com/MrSilaz/typo3snippets)
Visual Studio Code [Marketplace](https://marketplace.visualstudio.com/items?itemName=ralffreit.typo3snippets) 
        
## License

[GNU](http://www.gnu.org/licenses/gpl-2.0.html)
