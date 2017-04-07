# <a name="workbook-resource-type"></a>工作簿资源类型

工作簿是顶级对象，它包含相关 workbook 对象，例如工作表、表、范围等。

## <a name="properties"></a>属性
无

## <a name="relationships"></a>Relationships
| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|names|[NamedItem](nameditem.md) 集合|表示工作簿范围内的已命名项目（称为区域和常量）的集合。只读。|
|表格|[Table](table.md) 集合|表示与工作簿关联的表的集合。只读。|
|Worksheets|[Worksheet](worksheet.md) 集合|表示与工作簿关联的工作表的集合。只读。|

## <a name="functions"></a>函数

[Excel 函数](#functions)使用 JSON 对象调用使用语法 `POST /workbook/functions/{function-name}` 并在正文中提供函数自变量的工作簿函数。该函数产生 `value`，所有 `error` 字符串均返回到函数结果对象中。`null` 的 `error` 值表示该函数执行成功。 

受支持函数的完整列表在 [此处](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188)。请参阅特定参数名称和数据类型的函数签名。

_重要说明_： 
* 使用 range 对象（而不是范围地址字符串）提供范围输入参数。  
* 与大部分 API 中使用的从 0 开始的索引不同，索引参数从 1 开始索引。 

示例： 

在下面的示例中，通过传递查阅值、输入范围和要返回的值调用 `vlookup` 函数。 

请求： 

```http 
POST https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "lookupValue": "Temperature",
    "tableArray": { "Address": "Sheet1!E1:G5" },
    "colIndexNum": 2,
    "rangeLookup": false
}
```

响应：

```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

示例： 

在下面的示例中，通过传递数组中输入范围调用 `median` 函数。 

请求： 

```http 
POST https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"values" :  [
        { "address": "Sheet2!A1:A5" },
        { "address": "Sheet2!B1:B5" },
      ] 
}
```

响应：

```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "@odata.id": "/users('2abcad6a-2fca-4b6e-9577-e358a757d77d')/drive/root/workbook/functions/median()",
  "error": null,
  "value": 30
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
