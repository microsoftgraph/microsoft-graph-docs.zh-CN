# <a name="update-plannerplan"></a>更新 plannerplan

更新 **plannerplan** 对象的属性。
### <a name="prerequisites"></a>先决条件
要执行此 API，需要以下**范围**： 

*Group.ReadWrite.All*
### <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>
```
### <a name="optional-request-headers"></a>可选的请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer <code>|
| If-Match  | 要更新的 plannerPlan 的上次已知 ETag 值。必需。|

### <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|所有者|字符串|拥有计划的[组](../resources/group.md)`id`。必须存在有效的组才能设置此字段。设置后，只能由所有者更新此字段。|
|title|String|计划的标题。|

### <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerPlan](../resources/plannerplan.md) 对象。

此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。

### <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->