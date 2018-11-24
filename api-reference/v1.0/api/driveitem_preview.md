# <a name="driveitem-preview"></a>driveItem： 预览

此操作，可以获取项目的短期嵌入 Url 以便呈现临时预览。

如果您想要获取长生存期嵌入链接，请改用[createLink][] API。

> **注意：****预览**操作才当前 SharePoint 和 OneDrive for Business 上可用。

[createLink]: driveItem_createLink.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

| 权限类型                        | 权限（从最低特权到最高特权）
|:---------------------------------------|:-------------------------------------------
| 委派（工作或学校帐户）     | Files.Read，Files.ReadWrite，Files.ReadWrite.All Sites.ReadWrite.All
| 委派（个人 Microsoft 帐户） | Files.Read，Files.ReadWrite，Files.ReadWrite.All
| 应用程序                            | 不支持。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a>请求正文

在请求正文定义嵌入请求您的应用程序的 URL 的属性。
请求应为具有以下属性的 JSON 对象。

|   名称      |  类型         | 说明
|:------------|:--------------|:-----------------------------------------------
| page        | 字符串/编号 | 可选。 要启动，如果适用文档的页码。 指定为字符串的文件类型，如 ZIP 周围的将来使用情况。
| zoom        | number        | 可选。 如果适用，则缩放级别，从开始。

## <a name="response"></a>响应

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

响应将是一个 JSON 对象，包含以下属性：

| 名称           | 类型   | 说明
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | 适用于嵌入使用 HTTP GET （iframe 等） 的 URL
| postUrl        | string | 适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）
| postParameters | string | 如果使用 postUrl 包括 POST 参数

GetUrl、 postUrl，或同时可能会返回根据嵌入支持指定的选项的当前状态。

postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>页/缩放

页面和缩放选项可能适用于所有预览应用程序，但如果预览应用程序支持将应用。
