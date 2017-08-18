# <a name="move-a-driveitem"></a>移动 DriveItem

若要将 DriveItem 移动到新的父项，应用程序会请求更新要移动的 DriveItem 的 **parentReference**。这是[更新](item_update.md)方法的一种特殊情况。你的应用程序可以将以下操作组合到单个请求中：将项目移动到新的容器和更新项目的其他属性。

无法使用这一请求在 [驱动器](../resources/drive.md) 之间移动项目。

## <a name="prerequisites"></a>先决条件
要执行此 API，需要以下**范围**之一：

* Files.ReadWrite
* Files.ReadWrite.All
* Sites.ReadWrite.All


## <a name="http-request"></a>HTTP 请求

```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
```

## <a name="request-headers"></a>请求标头

| 名称          | 类型   | 说明                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | 如果包含此请求标头，且提供的 eTag（或 cTag）与文件夹上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。 |


## <a name="request-body"></a>请求正文
在请求正文中，提供 **parentReference** 属性的新值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

**注意：**将项目移动到 OneDrive 的根目录下时不能使用 `"id:" "root"` 语法。需要使用根文件夹的真实 ID，或对父引用使用 `{"path": "/drive/root"}`。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。

## <a name="example"></a>示例
本示例将 {item-id} 指定的项目移动到用户 OneDrive 的**文档**文件夹中。

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

##### <a name="response"></a>响应

以下示例显示了相应的响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
