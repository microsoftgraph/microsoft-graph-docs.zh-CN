# <a name="process-resource-type"></a>进程资源类型

包含有关与通知相关的进程的有状态信息。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|accountName|字符串|用户帐户标识符 （运行进程的用户帐户上下文），例如 AccountName、SID 等等。|
|commandLine|字符串|包括所有参数中的完整过程调用命令行。|
|createdDateTime|DateTimeOffset|进程开始的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|fileHash|[fileHash](filehash.md)|包含文件哈希 （加密和位置敏感）的复杂类型。|
|integrityLevel|processIntegrityLevel|过程的完整性级别。 可能的值为：`unknown`、`untrusted`、`low`、`medium`、`high`、`system`。|
|isElevated|布尔|如果提升进程，则为 true。|
|name|字符串|进程的图像文件的名称。|
|parentProcessCreatedDateTime|DateTimeOffset|父进程开始的日期时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|parentProcessId|Int32|父进程的进程 ID (PID) 。|
|parentProcessName|字符串|父进程的图像文件的名称。|
|path|字符串|完整路径，包括文件名。|
|processId|Int32|进程的进程 ID (PID)。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->