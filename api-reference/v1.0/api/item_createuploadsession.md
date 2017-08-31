# <a name="upload-large-files-with-an-upload-session"></a>通过上载会话上载大文件

通过创建上传会话，使应用可以上传最大大小的文件。上传会话使应用可以在连续的 API 请求中上传多个范围的文件，这样一来，如果在上传过程中连接断开，应用也可以继续传输文件。

若要使用上传会话上传文件，请执行以下两个步骤：

1. [创建上载会话](#create-an-upload-session)
2. [将字节上传到上传会话](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Sites.ReadWrite.All |

> **注意**：此 API 尚不支持 Files.ReadWrite.All 应用程序权限。即将规划提供完全支持。 

## <a name="create-an-upload-session"></a>创建上载会话

要开始上载大文件，你的应用程序必须先请求新的上载会话。这可以创建一个临时存储位置，在上载完成之前保存文件字节数。上载最后一个字节后，上载会话即完成，最终文件会出现在目标文件夹中。

### <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root:/{path-to-item}:/createUploadSession
POST /me/drive/items/{parent-item-id}:/{filename}:/createUploadSession
```

### <a name="request-body"></a>请求正文
不需要请求正文。但是，你可以指定请求正文，以便提供与正在上载的文件有关的其他数据。

例如，要控制是否已获得文件名的行为，可以在请求正文中指定冲突行为属性。

```json
{
    "item": {
        "@microsoft.graph.conflictBehavior": "rename"
    }
}
```

### <a name="optional-request-headers"></a>可选的请求标头

| 名称       | 值 | 说明                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *if-match* | etag  | 如果包含此请求标头，且提供的 eTag（或 cTag）与项目中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 错误响应。 |

### <a name="response"></a>响应
对此请求的响应将提供新建 [uploadSession](../resources/uploadsession.md) 的详细信息，其中包括用于上载部分文件的 URL。 

### <a name="example"></a>示例

<!-- {
  "blockType": "request",
  "name": "driveItem_createUploadSession"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createUploadSession
```

##### <a name="response"></a>响应 

以下示例显示了相应的响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://tenant-my.sharepoint.com/alkjl1kjklna",
  "expirationDateTime": "2020-08-24T10:58:00Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="upload-bytes-to-the-upload-session"></a>将字节上传到上传会话

若要上载文件或文件的一部分，你的应用程序可以对在 **createUploadSession** 响应中收到的 **uploadUrl** 值创建 PUT 请求。你可以上载整个文件，也可以将文件拆分为多个片段，只要任意给定请求的最大字节数少于 60 MiB 即可。必须按顺序上载文件的片段。不按顺序上载文件的片段将导致错误。

**注意：**如果应用程序将一个文件拆分成多个片段，则每个片段的大小**必须**是 320 KiB 的倍数。如果使用的片断大小不能被 320 整除，会导致在提交某些文件时出错。

### <a name="example"></a>示例

本示例将上载 128 字节大小的文件中的前 26 个字节。**Content-Length** 标头指定当前请求的大小。**Content-Range** 标头指定此请求表示的整个文件中的字节范围。必须先知道文件的总长度，然后才可以上载文件的第一个片段。

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

**重要说明：**应用程序必须确保 **Content-Range** 标头中指定的文件总大小对于所有的请求都相同。如果某片段声明有不同的文件大小，则请求将失败。

##### <a name="response"></a>响应

以下示例显示了相应的响应。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

应用程序可以使用 **nextExpectedRanges** 值来确定开始上载下一片段的位置。你可能会看到指定的多个范围，指示服务器尚未收到的文件部分。如果需要恢复中断的传输，并且客户端不能确定服务的状态，这个方法很有用。

始终都应根据以下最佳实践确定片段大小。请勿假定 **nextExpectedRanges** 将返回大小范围正确的上载片段。**nextExpectedRanges** 属性指定尚未收到的文件的范围，而不是上载文件的方式。

**注意：**

* `nextExpectedRanges` 属性不会总是列出所有缺少的范围。
* 成功写入片段时，它将返回下一个开始范围（例如，"523-"）。
* 如果因客户端发送了服务器已接收的片段导致失败，服务器将响应 `HTTP 416 Requested Range Not Satisfiable`。可以 [请求上载状态](#resuming-an-in-progress-upload) 以获取缺少范围的详细列表。
* 在发出 `PUT` 调用时添加授权标头可能会导致 `HTTP 401 Unauthorized` 响应。只能在第一步中发出 `POST` 时发送授权标头和持有者令牌。不得在发出 `PUT` 时添加授权标头。   


## <a name="completing-a-file"></a>完成文件

接收最后一个文件片段后，服务器将响应 `HTTP 201 Created` 或 `HTTP 200 OK`。响应正文还将包括 **driveItem** 的默认属性集，用来表示已完成的文件。

<!-- { "blockType": "request", "name": "upload-fragment-final", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 21
Content-Range: bytes 101-127/128

<final bytes of the file>
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```
**注意：**为使文档清晰起见，该项目的响应被截断。

## <a name="cancel-an-upload-session"></a>取消上载会话

若要取消上载会话，请将 DELETE 请求发送到上载 URL。这会清理用来保留以前上载的数据的临时文件。应在上载中止（例如，如果用户取消传输）的情况下使用上述方法。

**expirationDateTime** 通过后，系统将自动清理临时文件及其随附的上载会话。

### <a name="example"></a>示例

DELETE 请求将立即使上载会话过期，并删除以前上载的所有字节。

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->
```http
DELETE https://tenant-my.sharepoint.com/alkjl1kjklna
```

##### <a name="response"></a>响应 

以下示例显示了相应的响应。

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a>继续正在进行的上传

如果上载请求在完成前断开或失败，将忽略该请求中的所有字节。如果应用程序与服务之间的连接断开，可能会发生这种情况。如果发生这种情况，应用程序仍可以继续传输以前完成的文件片段。

若要查找以前已接收的字节范围，应用程序可以请求上载会话的状态。

### <a name="example"></a>示例
通过向 `uploadUrl` 发送 GET 请求来查询上载状态。

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->
```
GET https://tenant-my.sharepoint.com/alkjl1kjklna
```

服务器将用需要上载的缺失字节范围的列表和上载会话的过期时间进行响应。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a>上载剩余数据
现在，你的应用程序已经知道开始上载的位置，请按照 [将字节上载到上载会话](#upload-bytes-to-the-upload-session) 中的步骤继续上载。


## <a name="best-practices"></a>最佳实践

* 继续或重试由于连接中断或任意 5xx 错误而失败的上载，包括：
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* 如果在继续或重试上载请求时返回任意 5xx 服务器错误，请使用指数退避战略。
* 对于其他错误，不应使用指数退避战略，而应限制尝试重试的次数。
* 通过重新开始整个上载继续上载时，请处理 `404 Not Found` 错误。
* 对大于 10 MiB（10 \* 1024 \* 1024 字节）的文件使用可恢复文件传输。
* 最佳的文件片段大小是 10 MiB，可以实现稳定高速连接。对于速度较慢或不可靠的连接，较小的文件片段大小可能会给你带来更好的结果。建议使用的片段大小为 5-10 MiB 之间。
* 使用 320 KiB（320 \* 1024 字节）倍数的文件片段大小。如果使用的片段大小不是 320 KiB 的倍数，可能会在上载最后一个文件片段后导致大文件传输失败。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
