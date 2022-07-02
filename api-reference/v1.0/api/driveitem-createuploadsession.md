---
author: JeremyKelley
title: driveItem：createUploadSession
ms.localizationpriority: high
ms.prod: sharepoint
description: 通过创建上传会话，使应用可以上传最大大小的文件。
doc_type: apiPageType
ms.openlocfilehash: 5314c4060c72337d3a82821334f2e5d2bf0fe84f
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577887"
---
# <a name="driveitem-createuploadsession"></a>driveItem：createUploadSession

命名空间：microsoft.graph

通过创建上传会话，使应用可以上传最大大小的文件。上传会话使应用可以在连续的 API 请求中上传多个范围的文件，这样一来，如果在上传过程中连接断开，应用也可以继续传输文件。

若要使用上传会话上传文件，请执行以下两个步骤：

1. [创建上载会话](#create-an-upload-session)
2. [将字节上传到上传会话](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Sites.ReadWrite.All |

## <a name="create-an-upload-session"></a>创建上传会话

要开始上载大文件，你的应用程序必须先请求新的上载会话。
这可以创建一个临时存储位置，在上载完成之前保存文件字节数。
上载最后一个字节后，上载会话即完成，最终文件会出现在目标文件夹中。
或者，你可以通过在请求参数中设置 `deferCommit` 属性来推迟目标位置中的文件的最终创建，直到你显式发出完成上传的请求。

### <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a>请求正文

不需要任何请求正文。但是，你可以在请求正文中指定属性，以提供有关正在上传的文件的其他数据，并自定义上传操作的语义。

例如， `item` 属性允许设置以下参数：
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } -->
```json
{
  "@microsoft.graph.conflictBehavior": "fail (default) | replace | rename",
  "description": "description",
  "fileSize": 1234,
  "name": "filename.txt"
}
```

下面的示例控制文件名已被使用时的行为，并指定在发出显式完成请求之前，不应创建最终文件：

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  },
  "deferCommit": true
}
```

### <a name="optional-request-headers"></a>可选的请求标头

| 名称       | 值 | 说明                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *if-match* | etag  | 如果包含此请求标头，且提供的 eTag（或 cTag）与项目中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 错误响应。 |

## <a name="parameters"></a>参数

| 参数   | 类型                                                                           | 说明                                                                                           |
|:------------|:-------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------|
| deferCommit | 布尔值                                                                        | 如果设置为 `true`，则需要发出显式请求才能在目标中进行文件的最终创建。 |
| 项        | [driveItemUploadableProperties](../resources/driveItemUploadableProperties.md) | 有关正在上传的文件的数据。                                                                   |

### <a name="request"></a>请求

对此请求的响应将提供新建 [uploadSession](../resources/uploadsession.md) 的详细信息，其中包括用于上载部分文件的 URL。 

>**注意：**{item-path} 必须包含请求正文中指定的项的名称。

<!-- { "blockType": "request", "name": "upload-fragment-create-session", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/root:/{item-path}:/createUploadSession
Content-Type: application/json

{
  "item": {
    "@odata.type": "microsoft.graph.driveItemUploadableProperties",
    "@microsoft.graph.conflictBehavior": "rename",
    "name": "largefile.dat"
  }
}
```

### <a name="response"></a>响应

如果成功，此请求的响应将详细说明应将其余请求作为 [UploadSession](../resources/uploadsession.md) 资源发送到哪里。

此资源详细说明了应将文件的字节范围上传到哪里以及上传会话何时到期。

如果已指定 `fileSize` 参数，并且超出了可用配额，则将返回 `507 Insufficent Storage` 响应，并且不会创建上传会话。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession",
       "optionalProperties": [ "nextExpectedRanges" ]  } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z"
}
```

## <a name="upload-bytes-to-the-upload-session"></a>将字节上传到上传会话

若要上传文件或文件的一部分，你的应用程序可以对在 **createUploadSession** 响应中收到的 **uploadUrl** 值创建 PUT 请求。你可以上传整个文件，也可以将文件拆分为多个字节范围，只要任意给定请求的最大字节数少于 60 MiB 即可。

必须按顺序上传文件的片段。
不按顺序上载文件的片段将导致错误。

**注意：** 如果应用将一个文件拆分成多个字节范围，则每个字节范围的大小 **必须** 是 320 KiB（327,680 字节）的倍数。如果使用的片断大小不能被 320 KiB 整除，将导致在提交某些文件时出错。

### <a name="example"></a>示例

在本示例中，应用将上传 128 字节大小的文件中的前 26 个字节。

* **Content-Length** 标头指定当前请求的大小。
* **Content-Range** 标头指示此请求表示的整个文件中的字节范围。
* 要先知道文件的总长度，然后才可以上传文件的第一个片段。

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

**重要说明：** 应用程序必须确保 **Content-Range** 标头中指定的文件总大小对于所有的请求都相同。如果某字节范围声明有不同的文件大小，则请求将失败。

### <a name="response"></a>响应

当此请求完成时，如果还需要上传其他字节范围，服务器将会返回 `202 Accepted` 作为响应。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

你的应用程序可以使用 **nextExpectedRanges** 值来确定开始上传下一字节范围的位置。你可能会看到指定的多个范围，指示服务器尚未收到的文件部分。如果需要恢复中断的传输，并且客户端不能确定服务的状态，这个方法很有用。

始终都应根据以下最佳实践确定字节范围大小。请勿假定 **nextExpectedRanges** 将返回大小范围正确的上传字节范围。**nextExpectedRanges** 属性指定尚未收到的文件的范围，而不是应用上传文件的方式。

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": [
  "12345-55232",
  "77829-99375"
  ]
}
```

## <a name="remarks"></a>备注

* `nextExpectedRanges` 属性不会总是列出所有缺少的范围。
* 成功写入片段时，它将返回下一个开始范围（例如，"523-"）。
* 如果因客户端发送了服务器已接收的片段导致失败，服务器将响应 `HTTP 416 Requested Range Not Satisfiable`。可以 [请求上载状态](#resuming-an-in-progress-upload) 以获取缺少范围的详细列表。
* 在发出 `PUT` 调用时添加授权标头可能会导致 `HTTP 401 Unauthorized` 响应。只能在第一步中发出 `POST` 时发送授权标头和持有者令牌。不得在发出 `PUT` 时添加授权标头。

## <a name="completing-a-file"></a>完成文件

如果 `deferCommit` 为 false 或未设置，则在将文件的最终字节范围放入上传 URL 时，将自动完成上传。

如果 `deferCommit` 为 true，则可通过以下两种方式显式完成上传：
- 将文件的最终字节范围放入上传 URL 后，将最终的 POST 请求发送到内容长度为零的上传 URL（当前仅在 OneDrive for Business 和 SharePoint 中受支持）。
- 将文件的最终字节范围放入上传 URL 后，以[处理上传错误](#handle-upload-errors)的相同方式发送最终 PUT 请求（目前仅在 OneDrive Personal 中受支持）。


当完成上传后，服务器将使用 `HTTP 201 Created` 或 `HTTP 200 OK` 来响应最终请求。响应正文还将包括 **driveItem** 的默认属性集，用来表示已完成的文件。

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "files.readwrite" } -->

```
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
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

<!-- { "blockType": "request", "opaqueUrl": true, "name": "commit-upload", "scopes": "files.readwrite" } -->

```http
POST https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 0
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


## <a name="handling-upload-conflicts"></a>处理上传冲突

如果在文件上传后发生冲突（例如，在上传会话期间创建了同名的项），则会在最后一个字节范围上传时返回错误。

```http
HTTP/1.1 409 Conflict
Content-Type: application/json

{
  "error":
  {
    "code": "upload_name_conflict",
    "message": "Another file exists with the same name as the uploaded session. You can redirect the upload session to use a new filename by calling PUT with the new metadata and @microsoft.graph.sourceUrl attribute.",
  }
}
```

## <a name="cancel-the-upload-session"></a>取消上传会话

若要取消上载会话，请将 DELETE 请求发送到上载 URL。这会清理用来保留以前上载的数据的临时文件。应在上载中止（例如，如果用户取消传输）的情况下使用上述方法。

**expirationDateTime** 通过后，系统将自动清理临时文件及其随附的上传会话。
有效期过后可能不会立即删除临时文件。

### <a name="request"></a>请求

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a>响应

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

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```http
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

服务器将用需要上载的缺失字节范围的列表和上载会话的过期时间进行响应。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a>上载剩余数据

现在，你的应用程序已经知道开始上载的位置，请按照 [将字节上载到上载会话](#upload-bytes-to-the-upload-session) 中的步骤继续上载。

## <a name="handle-upload-errors"></a>处理上传错误

在上传文件的最后一个字节范围时，可能会出现错误。这可能是由于名称冲突或超出配额限制所致。将保留未到期的上传会话，这允许应用通过显式提交上传会话来恢复上传。

若要显式提交上传会话，应用必须使用将用来提交上传会话的新 **driveItem** 资源发出 PUT 请求。
此新请求应纠正生成原始上传错误的错误根源。

若要指示应用提交现有上传会话，PUT 请求必须包含 `@microsoft.graph.sourceUrl` 属性以及上传会话 URL 的值。

<!-- { "blockType": "ignored", "name": "explicit-upload-commit", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PUT /me/drive/root:/{path_to_parent}
Content-Type: application/json
If-Match: {etag or ctag}

{
  "name": "largefile.vhd",
  "@microsoft.graph.conflictBehavior": "rename",
  "@microsoft.graph.sourceUrl": "{upload session URL}"
}
```

>**注意：** 可以在此调用中正常使用 `@microsoft.graph.conflictBehavior` 和 `if-match` 头。

### <a name="response"></a>响应

如果可以使用新的元数据提交文件，将返回 `HTTP 201 Created` 或 `HTTP 200 OK` 响应，其中包含已上传文件的项元数据。

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

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

## <a name="best-practices"></a>最佳做法

* 继续或重试由于连接中断或任意 5xx 错误而失败的上载，包括：
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* 如果在继续或重试上载请求时返回任意 5xx 服务器错误，请使用指数退避战略。
* 对于其他错误，不应使用指数退避战略，而应限制尝试重试的次数。
* 通过重新开始整个上传继续上传时，请处理 `404 Not Found` 错误。 这表示上传会话不再存在。
* 对大于 10 MiB（10,485,760 个字节）的文件使用可恢复文件传输。
* 最佳的字节范围大小是 10 MiB，可以实现稳定高速连接。对于速度较慢或不可靠的连接，较小的文件片段大小可能会给你带来更好的结果。建议使用的片段大小为 5-10 MiB 之间。
* 使用 320 KiB（327,680 个字节）倍数的字节范围大小。 如果使用的片段大小不是 320 KiB 的倍数，可能会在上传最后一个字节范围后导致大文件传输失败。

## <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]主题，详细了解错误返回方式。

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

## <a name="see-also"></a>另请参阅

[大文件上传](/graph/sdks/large-file-upload)

<!-- {
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "suppressions": [
  ],
  "section": "documentation"
} -->

