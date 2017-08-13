# <a name="update-a-group-setting"></a>更新组设置

更新特定组设置对象的属性。

## <a name="prerequisites"></a>先决条件

要执行此 API，需要以下**范围**之一：*Directory.ReadWrite.All* 或 *Directory.AccessAsUser.All*

> 注意：只有租户管理员有权执行创建、更新和删除操作。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->

更新租户范围或组特定设置。

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a>可选的请求标头
| 名称 | 说明 |
|:-----------|:-----------|
| Authorization  | Bearer {token}。必需。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。 

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| values | settingValue | 更新的值集。注意：必须提供整个集合组。无法更新单个值集合。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `204 OK` 响应代码和更新的 [groupSetting](../resources/groupsetting.md) 对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->