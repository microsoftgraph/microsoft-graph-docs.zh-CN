# <a name="get-directory-objects-from-a-list-of-ids"></a>获取 ID 列表中的目录对象

返回 ID 列表中指定的目录对象。注意：返回的目录对象是包含其**所有**属性的完整对象。`$select` 查询选项不适用于此操作。

该函数的一些常见用途是：

* 将返回 ID 集合的函数（例如 [getMemberObjects](directoryobject_getmemberobjects.md) 或 [getMemberGroups](directoryobject_getmembergroups.md)）返回的 ID 解析到其后备目录对象。
* 将应用程序保存在外部存储的 ID 解析到其后备目录对象。

## <a name="prerequisites"></a>先决条件

要执行此 API，需要以下**范围**之一：_Directory.Read.All_；_Directory.AccessAsUser.All_

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getById
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | 持有者&lt;令牌&gt;。必需。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数   | 类型 |说明|
|:---------------|:--------|:----------|
|ids|String collection| 要返回其对象的 ID 集合。最多可以指定 1000 个 ID。 |
|types|String collection| 指定要搜索的资源集合集的资源类型集合。如果未指定，则默认为 [directoryObject](../resources/directoryobject.md)，其包含目录中定义的所有资源类型。可以在该集合中指定派生自 `directoryObject` 的所有对象，例如：[用户](../resources/user.md)、[组](../resources/group.md)、[设备](../resources/device.md)等。这些值不区分大小写。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 String 集合对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a>响应

注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
