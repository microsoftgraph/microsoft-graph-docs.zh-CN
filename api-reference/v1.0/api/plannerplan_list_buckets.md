# <a name="list-buckets"></a>列出存储桶

检索 [plannerPlan](../resources/plannerplan.md) 对象包含的 **plannerbucket** 对象列表。
## <a name="prerequisites"></a>先决条件
要执行此 API，需要以下**范围**： 

*Group.Read.All*
## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>/buckets
```

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
### <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerBucket](../resources/plannerbucket.md) 对象集合。

此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/2txjA-BMZEq-bKi6Wfj5aGQAB1OJ/buckets
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->