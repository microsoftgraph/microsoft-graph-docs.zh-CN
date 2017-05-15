# <a name="workbookpivottable-refreshall"></a>workbookPivotTable: refreshAll

刷新给定工作表中的数据透视表。

### <a name="prerequisites"></a>先决条件
若要执行此 API，必须有以下**范围**：_Files.Read、Files.ReadWrite_
### <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
### <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Workbook-Session-Id  | 确定是否保留更改的工作簿会话 ID。可选。|

### <a name="request-body"></a>请求正文

### <a name="response"></a>响应
如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。

### <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
