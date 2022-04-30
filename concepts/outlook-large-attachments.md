---
title: 将大文件附加到 Outlook 邮件或事件
description: 可选择两种方法中的一种来将文件附加到邮件或事件，具体取决于文件的大小。
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 582501205c106b3deaf0312f3db9c81488feb3de
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133046"
---
# <a name="attach-large-files-to-outlook-messages-or-events"></a>将大文件附加到 Outlook 邮件或事件

使用 Microsoft Graph API，可将最大 150 MB 的文件附加到 Outlook [邮件](/graph/api/resources/message)或 [事件](/graph/api/resources/event)项目。 根据文件大小，选择以下两种方法之一来附加文件：
- 如果文件大小小于 3 MB，请对 Outlook 项目的 **附件** 导航属性执行单个 POST; 了解如何 [为邮件或](/graph/api/message-post-attachments) 或 [为事件](/graph/api/event-post-attachments) 执行此操作。成功的 `POST` 响应包括文件附件的 ID。
- 如果文件大小介于 3MB 到 150MB 之间，请创建上传会话，并迭代使用 `PUT` 上传文件的字节范围，直到上传整个文件为止。最终成功的 `PUT` 响应中的标头包括包含附件 ID 的 URL。

若要将多个文件附加到邮件，请根据每个文件的文件大小，选择相应的方法，并单独附加文件。

本文逐步介绍了第二种方法，创建并使用上传会话来添加大型文件附件（大小超过 3 MB）至 Outlook 项。 各步显示相应的邮件或事件代码。 成功上传整个文件后，文章显示获取含有文件附件 ID 的响应标头，随后显示使用附件 ID 来获取原始附件内容或附件元数据。 

> [!IMPORTANT] 
> 如果要将大文件附加到共享或委派邮箱中的邮件或事件，请注意一个[已知问题](known-issues.md#attaching-large-files-to-messages-with-delegated-permissions-can-fail)。

## <a name="step-1-create-an-upload-session"></a>第 1 步：创建上传会话

[创建上传会话](/graph/api/attachment-createuploadsession)，将文件附加到邮件或事件。 在输入参数 **AttachmentItem** 中指定文件。

成功的操作返回 `HTTP 201 Created` 和新的 [uploadSession](/graph/api/resources/uploadsession) 实例，其中包含可在后续 `PUT` 操作中用于上传文件各部分的非跳转 URL。 **uploadSession** 提供一个临时存储位置，在此位置保存文件字节数，直到完整文件上传完毕。

响应中的 **uploadSession** 对象还包含 **nextExpectedRanges** 属性，这表明初始上传开始位置应该为 0 字节。

### <a name="permissions"></a>权限
请务必请求 `Mail.ReadWrite` 权限，以为邮件创建 **uploadSession**，并为事件创建 `Calendars.ReadWrite`。 

新的 **uploadSession** 的 **uploadUrl** 属性中返回的非跳转 URL 经过预身份验证，包含针对 `https://outlook.office.com` 域中后续 `PUT` 查询的相应授权令牌。 该令牌会在 **expirationDateTime** 过期。 请勿自定义 `PUT` 操作的此 URL。


### <a name="example-create-an-upload-session-for-a-message"></a>示例：创建邮件的上传会话

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession_message",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/walkthrough-create-uploadsession-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下列示例响应显示为邮件返回的 **uploadSession** 资源。

<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

### <a name="example-create-an-upload-session-for-an-event"></a>示例：创建事件的上传会话
#### <a name="request"></a>请求 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "walkthrough_create_uploadsession_event",
  "sampleKeys": ["AAMkADU5CCmSAAA="]
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkADU5CCmSAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/walkthrough-create-uploadsession-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/walkthrough-create-uploadsession-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/walkthrough-create-uploadsession-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/walkthrough-create-uploadsession-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
下列示例响应显示为shi'jian事件返回的 **uploadSession** 资源。

<!-- {
  "blockType": "response",
  "name": "walkthrough_create_uploadsession_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw",
    "expirationDateTime": "2020-02-22T02:46:56.7410786Z",
    "nextExpectedRanges": [
        "0-"
    ]
}

```


## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a>步骤 2：使用上传会话上传文件的字节范围

如果要上传文件或文件的一部分，在 **uploadSession** 资源 **uploadUrl** 属性中，对第 1 步返回的 URL 进行 `PUT` 请求。 可上传整个文件，或将文件拆分为多个字节范围。 为获得更好的性能，请保持每个字节范围小于 4 MB。

按如下所述指定请求标头和请求正文。

### <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Content-Length | Int32 | 此操作中上传的字节数。 为获得更好的性能，请将每个 `PUT` 操作的字节数的上限限制为 4 MB。 必填。 |
| Content-Range | 字符串 | 在此操作中上传文件的基于 0 的字节范围，用格式 `bytes {start}-{end}/{total}` 表示。必填。 |
| Content-Type | String  | MIME 类型。 指定 `application/octet-stream`。 必填。 |

请勿指定 `Authorization` 请求标头。 `PUT` 查询使用 **uploadUrl** 属性中的预身份验证 URL，该 URL 允许访问 `https://outlook.office.com` 域。

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

### <a name="example-first-upload-to-the-message"></a>示例：首先上传至消息
#### <a name="request"></a>请求
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>响应

下列示例响应在 **NextExpectedRanges** 属性中显示服务器预期的下一字节范围的起点。
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://outlook.office.com/api/v2.0/$metadata#Users('a8e8e219-4931-95c1-b73d-62626fd79c32%4072aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA%3D')/AttachmentSessions/$entity",
  "ExpirationDateTime":"2019-09-25T01:09:30.7671707Z",
  "NextExpectedRanges":["2097152"]
}
```

### <a name="example-first-upload-to-the-event"></a>示例：首先上传至事件
#### <a name="request"></a>请求
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>响应

下列示例响应在 **NextExpectedRanges** 属性中显示服务器预期的下一字节范围的起点。
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://outlook.office.com/api/v2.0/$metadata#Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69%4098a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA%3D')/AttachmentSessions/$entity",
    "ExpirationDateTime":"2020-02-22T02:46:56.7410786Z",
    "NextExpectedRanges":["2097152"]
}
```


## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a>步骤 3：继续上传字节范围，直至完整文件上传完毕

执行步骤 2 中的初始上传后，在会话的到期日期/时间前，使用步骤 2 中所述的 `PUT` 请求，继续上传文件中剩余的部分。 使用 **NextExpectedRanges** 集合确定要上传的下一个字节范围的开头。 可能会发现指定了多个范围，这些范围指明了服务器尚未收到的文件部分。 如果需要恢复中断的传输，并且客户端不能确定服务的状态，这个方法很有用。

成功上传文件的最后一个字节后，最终 `PUT` 操作返回 `HTTP 201 Created` 以及指示 `https://outlook.office.com` 域中文件附件 URL 的 `Location` 标头。 可从 URL 获取附件 ID 并将其保存供以后使用。 可以使用该 ID [获取附件的元数据](/graph/api/attachment-get)，或使用 Microsoft Graph 终结点[将附件从 Outlook 项中删除](/graph/api/attachment-delete)，具体取决于你的场景。

下列示例显示在此处理步骤中上传最后的文件字节范围至邮件和事件。

### <a name="example-final-upload-to-the-message"></a>示例：最后上传至消息
#### <a name="request"></a>请求
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>响应
下列示例显示可保存附件 ID（`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`）以供随后使用的 `Location` 响应标头。

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')
Content-Length: 0
```

### <a name="example-final-upload-to-the-event"></a>示例：最后上传至事件
#### <a name="request"></a>请求
<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/AttachmentSessions('AAMkADU5RpAACJlCs8AAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIBtw
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>响应
下列示例显示可保存附件 ID（`AAMkADU5CCmSAAANZAlYPeyQByv7Y=`）以供随后使用的 `Location` 响应标头。

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://outlook.office.com/api/v2.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')
Content-Length: 0
```

## <a name="step-4-optional-get-the-file-attachment-from-the-outlook-item"></a>步骤 4（可选）：从 Outlook 项中获取文件附件

和往常一样，从 Outlook 项中[获取附件](/graph/api/attachment-get)在理论上并不受附件大小限制。

但是，获取采用 base64 编码格式的大文件附件会影响 API 性能。 如果需要大型附件：

- 作为获取采用 base64 格式的附件内容的替代方法，可以[获取文件附件的元数据](/graph/api/attachment-get#example-6-get-the-raw-contents-of-a-file-attachment-on-a-message)。
- 要 [获取文件附件的元数据](/graph/api/attachment-get#example-1-get-the-properties-of-a-file-attachment)，可以附加 `$select` 参数以仅包含所需的元数据属性，排除返回采用 base64 格式的文件附件的 **contentBytes** 属性。

### <a name="example-get-the-raw-file-attached-to-the-event"></a>示例：获取附加到事件的原始文件
按照事件示例和使用 `Location` 上一步标头中返回的附件 ID，此部分中的示例请求显示了使用 `$value` 参数获取附件的原始内容数据。

#### <a name="permissions"></a>权限
对于此操作，请根据需要使用最小特权委派或应用程序权限 `Calendars.Read`。有关详细信息，请参阅 [日历权限](permissions-reference.md#calendars-permissions)。

#### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "sampleKeys": ["d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32", "AAMkADU5CCmSAAA=", "AAMkADU5CCmSAAANZAlYPeyQByv7Y="]
}-->
```http
GET https://graph.microsoft.com/v1.0/Users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69@98a79ebe-74bf-4e07-a017-7b410848cb32')/Events('AAMkADU5CCmSAAA=')/Attachments('AAMkADU5CCmSAAANZAlYPeyQByv7Y=')/$value
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "ignored",
  "name": "walkthrough_get_attachment_raw",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
content-length: 3483322
Content-type: image/jpeg

{Raw bytes of the file}
```


### <a name="example-get-the-metadata-of-the-file-attached-to-the-message"></a>示例：获取邮件附加的文件的元数据
按照邮件示例，此部分中的示例请求显示使用 `$select` 参数来获取有关邮件的文件附件的部分元数据，不包括 **contentBytes**。

#### <a name="permissions"></a>权限
对于此操作，请根据需要使用最小特权委派或应用程序权限 `Mail.Read`。有关详细信息，请参阅 [邮件权限](permissions-reference.md#mail-permissions)。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "walkthrough_get_attachment_metadata",
  "sampleKeys": ["a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47", "AAMkADI5MAAIT3drCAAA=", "AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0="]
}-->
```http
GET https://graph.microsoft.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/Attachments('AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=')?$select=lastModifiedDateTime,name,contentType,size,isInline
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "walkthrough_get_attachment_metadata",
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
    "isInline": false
}
```


## <a name="alternative-cancel-the-upload-session"></a>替代方法：取消上传会话

在上传会话过期之前的任何时间点，如果必须取消上传，可以使用相同的初始不透明 URL 删除上传会话。成功的操作返回 `HTTP 204 No Content`。

### <a name="permissions"></a>权限
由于初始不透明的 URL 为预验证，并包含该上传会话后续查询的适当授权令牌，所以请勿为此操作指定授权请求标题。

### <a name="example-cancel-the-upload-session-for-the-message"></a>示例：取消邮件的上传会话

#### <a name="request"></a>请求
<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://outlook.office.com/api/v2.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0tAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```
## <a name="errors"></a>错误

### <a name="errorattachmentsizeshouldnotbelessthanminimumsize"></a>ErrorAttachmentSizeShouldNotBeLessThanMinimumSize

尝试[创建上传会话](/graph/api/attachment-createuploadsession)以附加小于 3 MB 的文件时返回此错误。 如果文件大小小于 3 MB，则应该针对 [邮件](/graph/api/message-post-attachments)或 [事件](/graph/api/event-post-attachments)的 **附件** 导航属性执行单个 POST。 成功的 `POST` 响应包括附加到邮件的文件的 ID。

