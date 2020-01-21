---
title: 将大文件附加到 Outlook 邮件
description: 可选择两种方法中的一种来将文件附加到邮件，具体取决于文件的大小。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 4b6aaa2e10ac1fc718d306921dab60b771c8b9e4
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216852"
---
# <a name="attach-large-files-to-outlook-messages-as-attachments-preview"></a>将大文件作为附件附加到 Outlook 邮件（预览）

可选择两种方法中的一种来将文件附加到[邮件](/graph/api/resources/message?view=graph-rest-beta)，具体取决于文件的大小：

- 如果文件大小小于 4 MB，则可以[针对邮件的附件导航属性执行单个 POST](/graph/api/message-post-attachments?view=graph-rest-beta)。 成功的 `POST` 响应包括附加到邮件的文件的 ID。
- 如果文件大小介于 3MB 和 150MB 之间，则创建一个上传会话，并以迭代的方式使用 `PUT` 来上传文件的字节范围，直到完整的文件上传完毕。 最后一个成功 `PUT` 响应中的标头包括带附件 ID 的 URL。 

本文使用一个示例来阐释第二种方法。 该示例创建并使用上传会话，将大文件附件（大小超过 3MB）添加到特定邮件。 成功上传整个文件时，它会获取一个 URL，其中包含文件附件的 ID，可用于执行其他操作，如获取文件附件元数据。

## <a name="step-1-create-an-upload-session"></a>第 1 步：创建上传会话

[创建上传会话](/graph/api/attachment-createuploadsession?view=graph-rest-beta)，将文件附加到邮件。 在输入参数 **AttachmentItem** 中指定文件。 

成功的操作返回 `HTTP 201 Created` 和新的 [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta) 实例，其中包含可在后续 `PUT` 操作中用于上传文件各部分的非跳转 URL。 **uploadSession** 提供一个临时存储位置，在此位置保存文件字节数，直到完整文件上传完毕。 

请务必请求 `Mail.ReadWrite` 权限以创建 **uploadSession**。 新的 **uploadSession** 的 **uploadUrl** 属性中返回的非跳转 URL 经过预身份验证，包含针对 `https://outlook.office.com` 域中后续 `PUT` 查询的相应授权令牌。 该令牌会在 **expirationDateTime** 过期。 请勿自定义 `PUT` 操作的此 URL。

响应中的 **uploadSession** 对象还包含 **nextExpectedRanges** 属性，这指示初始上传开始位置应该为 0 字节。

### <a name="example-request-create-an-upload-session"></a>示例请求：创建上传会话

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower", 
    "size": 3483322
  }
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="example-response-get-an-uploadsession-object"></a>示例响应：获取 uploadSession 对象
<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a>步骤 2：使用上传会话上传文件的字节范围

要上传文件或文件的一部分，请向作为步骤 1 中 **uploadSession** 一部分返回的 **uploadUrl** 属性发出 `PUT` 请求。 可上传整个文件，或将文件拆分为多个字节范围。 为获得更好的性能，请保持每个字节范围小于 4 MB。 

按如下所述指定请求标头和请求正文。

### <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Content-Length | Int32 | 此操作中上传的字节数。 为获得更好的性能，请将每个 `PUT` 操作的字节数的上限限制为 4 MB。 必填。 |
| Content-Range | 字符串 | 此操作中要上传的文件的从 0 开始的字节范围，格式为 `bytes {start}-{end}/{total}`。 必填。 |
| Content-Type | String  | MIME 类型。 指定 `application/octet-stream`。 必填。 |

请勿指定 `Authorization` 请求标头。 `PUT` 查询使用 **uploadUrl** 属性中预身份验证的 URL，该属性允许访问 `https://outlook.office.com` 域。

### <a name="request-body"></a>请求正文

指定要附加的文件的实际字节数，它们位于由 `Content-Range` 请求标头指定的位置范围内。

### <a name="response"></a>响应
成功的上传将返回 `HTTP 200 OK` 和 **uploadSession** 对象。 请注意响应对象中的以下项：

- **ExpirationDateTime** 属性指示 **uploadUrl** 属性值中嵌入的身份验证令牌的到期日期/时间。 此到期日期/时间与步骤 1 中由初始 **uploadSession** 返回的值相同。 
- **NextExpectedRanges** 指定上传开始的下一个字节位置，例如 `"NextExpectedRanges":["2097152"]`。 必须按顺序上传文件中的字节。
<!-- The **NextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"NextExpectedRanges":["2097152"]`. 
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"NextExpectedRanges":["1998457-2097094"]`.
-->
- **uploadUrl** 属性不会显式返回，因为上传会话的所有 `PUT` 操作使用创建会话时返回的同一 URL（步骤 1）。

### <a name="example-request-first-upload"></a>示例请求：第一次上传
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

### <a name="example-response-get-the-start-of-the-next-byte-range-that-the-server-expects"></a>示例响应：获取服务器需要的下一个字节范围的开头
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://outlook.office.com/api/beta/$metadata#Users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA%3D')/AttachmentSessions/$entity",
  "ExpirationDateTime":"2019-09-25T01:09:30.7671707Z",
  "NextExpectedRanges":["2097152"]
}
```


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a>步骤 3：继续上传字节范围，直至完整文件上传完毕

执行步骤 2 中的初始上传后，在会话的到期日期/时间前，使用步骤 2 中所述的 `PUT` 请求，继续上传文件中剩余的部分。 使用 **NextExpectedRanges** 集合确定要上传的下一个字节范围的开头。 可能会发现指定了多个范围，这些范围指明了服务器尚未收到的文件部分。 如果需要恢复中断的传输，并且客户端不能确定服务的状态，这个方法很有用。

成功上传文件的最后一个字节后，最终 `PUT` 操作返回 `HTTP 201 Created` 以及指示 `https://outlook.office.com` 域中文件附件 URL 的 `Location` 标头。 可从 URL 获取附件 ID 并将其保存供以后使用。 可以使用该 ID [获取附件的元数据](/graph/api/attachment-get?view=graph-rest-beta)，或使用 Microsoft Graph 终结点[将附件从邮件中删除](/graph/api/attachment-delete?view=graph-rest-beta)，具体取决于你的场景。

以下示例显示上传文件的最后一个字节范围。

### <a name="example-request-final-upload"></a>示例请求：最后一次上传
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

### <a name="example-response-get-the-location-response-header-to-save-the-attachment-id"></a>示例响应：获取位置响应标头以保存附件 ID

通过 `Location` 响应标头指定的 URL，保存附件 ID (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) 以便日后使用。

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-message"></a>步骤 4（可选）：从邮件中获取文件附件

和往常一样，从邮件中[获取附件](/graph/api/attachment-get?view=graph-rest-beta)在理论上并不受附件大小限制。 

但是，获取采用 base64 编码格式的大文件附件会影响 API 性能。 如果需要大型附件：
 
- 作为获取采用 base64 格式的附件内容的替代方法，可以[获取文件附件的元数据](/graph/api/attachment-get#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message?view=graph-rest-1.0)。
- 要[获取文件附件的元数据](/graph/api/attachment-get?view=graph-rest-beta#example-1-get-the-properties-of-a-file-attachment)，可以附加 `$select` 参数以仅包含所需的元数据属性，排除返回采用 base64 格式的文件附件的 **contentBytes** 属性。

### <a name="example-request-get-the-file-attachment-metadata"></a>示例请求：获取文件附件元数据

下面的示例显示发件人使用 `$select` 参数获取邮件中文件附件的所有元数据，除了 **contentBytes**。

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment", 
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline,contentId,contentLocation
```

### <a name="example-response"></a>示例响应

<!-- {
  "blockType": "response",
  "name": "walkthrough_get_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/messages('AAMkADI5MAAIT3drCAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "@odata.mediaContentType": "image/jpeg",
    "id": "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=",
    "lastModifiedDateTime": "2019-09-24T23:27:43Z",
    "name": "flower",
    "contentType": "image/jpeg",
    "size": 3640066,
    "isInline": false,
    "contentId": null,
    "contentLocation": null
}
```

## <a name="alternative-cancel-the-upload-session"></a>替代方法：取消上传会话

在上传会话到期之前的任何时间，如果必须取消上传，可使用同一初始非跳转 URL 来删除上传会话。 成功的操作将返回 `HTTP 204 No Content`。

### <a name="example-request-cancel-an-upload-session"></a>示例请求：取消上传会话

<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

### <a name="example-response"></a>示例响应

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```


