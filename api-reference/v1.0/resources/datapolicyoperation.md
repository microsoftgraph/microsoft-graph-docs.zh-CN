# <a name="datapolicyoperation-resource-type"></a>dataPolicyOperation 资源类型

代表提交的数据策略操作。 它包含跟踪操作的状态所需的信息。 例如，公司管理员可以提交数据策略操作请求员工的公司数据导出，然后更高版本跟踪该请求。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |检索**dataPolicyOperation**对象的属性。|
|[导出个人数据](../api/user-exportpersonaldata.md) | 无 |提交数据策略操作请求，以便以后可以使用[获取 dataPolicyOperation](../api/datapolicyoperation-get.md)读取的组织用户的数据导出|

## <a name="properties"></a>属性

> **注意：** 此资源的所有属性都是只读的。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|表示此数据策略操作的请求完成时，在 UTC 时间中，使用 ISO 8601 格式。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 在操作完成前，则为 null。|
|id|String| 此操作的唯一键。 |
|状态|string| 可取值为：`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。|
|storageLocation|String|到要从中导出数据的导出请求的 URL 位置。|
|userId|String|在其执行操作的用户 id。|
|submittedDateTime|DateTimeOffset|表示此数据操作的请求已提交时，在 UTC 时间中，使用 ISO 8601 格式。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|进度|String|指定操作的进度。|

## <a name="relationships"></a>关系
无。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)", 
  "progress": "String (double)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
