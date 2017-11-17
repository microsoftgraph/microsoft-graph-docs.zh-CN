# <a name="uploadsession-resource-type"></a>UploadSession 资源类型

**UploadSession** 资源提供了有关如何将大文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库的信息。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "expirationDateTime": "timestamp",
  "nextExpectedRanges": ["string"],
  "uploadUrl": "url"
}

```
## <a name="properties"></a>属性


| 属性             | 类型              |说明|
|:-------------------|:------------------|:----------|
| expirationDateTime | DateTimeOffset    | 以 UTC 表示的上载会话过期的日期和时间。在此过期时间之前必须上载完整的文件文件。 |
| nextExpectedRanges | String collection | 字节范围集合，文件服务器缺失。这些区域索引均从零开始，格式为“开始-结束”（例如，“0-26”指示该文件的前 27 个字节)。 |
| uploadUrl          | String            | 接受文件字节范围的 PUT 请求的 URL 端点。 |

## <a name="additional-resources"></a>其他资源

有关如何使用上载会话上载文件的详细信息，请参阅 [使用上载会话上载大文件](../api/item_createUploadSession.md)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "uploadSession resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->