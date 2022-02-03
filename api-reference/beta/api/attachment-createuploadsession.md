---
title: attachment： createUploadSession
description: 创建上载会话以迭代上载文件的范围，以便将文件附加到指定消息。
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3a36f5e3e41caebdde8f1c8f80356980d1a470e5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340372"
---
# <a name="attachment-createuploadsession"></a>attachment： createUploadSession

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建允许应用迭代上载文件范围的上载会话，以便将文件附加到Outlook项。 项目可以是消息[或](../resources/message.md)[事件](../resources/event.md)。

如果文件大小在 3 MB 到 150 MB 之间，则使用该方法附加文件。 若要附加小于 3 MB `POST` 的文件，请对 Outlook 项目的 **attachments** 导航属性执行一个操作;请参阅如何为邮件或 [事件执行该操作](event-post-attachments.md)。[](message-post-attachments.md) 

作为响应的一部分，此操作返回可用于后续顺序查询的上载 `PUT` URL。 通过每个操作的请求 `PUT` 标头，可以指定要上载的字节的准确范围。 这允许恢复传输，以防在上载过程中网络连接中断。 

以下是使用上载会话将文件附加到Outlook项的步骤：

1. 创建上载会话。
2. 在上载会话内， (上载字节范围，每次) 最多上载 4 MB，直到上载文件的所有字节，并且文件附加到指定项。
3. 保存附件的 ID，供将来访问。
4. 可选：删除上载会话。

有关[示例，请参阅Outlook大文件附加到邮件](/graph/outlook-large-attachments)或事件。

> [!TIP]
> Exchange Online管理员可自定义邮箱的邮件大小Microsoft 365包括任何邮件附件。 默认情况下，此邮件大小限制为 35 MB。 了解如何自定义 [最大邮件大小](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) 以支持大于租户默认限制的附件。 

> [!IMPORTANT] 
> 如果要将大 [文件附加到](/graph/known-issues#attaching-large-files-to-messages) 共享或委派邮箱中的邮件或事件，请注意已知问题。


## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Mail.ReadWrite |
| 委派（个人 Microsoft 帐户） | Mail.ReadWrite |
| 应用程序                            | Mail.ReadWrite |

## <a name="http-request"></a>HTTP 请求

若要创建上载会话以将文件附加到 **事件**： 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

若要创建用于将文件附加到邮件的上载 **会话，** 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 {token} |


## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型        | 说明 |
|:-------------|:------------|:------------|
|AttachmentItem|[attachmentItem](../resources/attachmentitem.md)|表示要上载和附加的项目的属性。 至少应指定附件 (`file`) 、名称和文件大小。|

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和新 [uploadSession](../resources/uploadsession.md) 对象。

>**注意**： 
>
>作为 **uploadSession** 响应`PUT`对象的一部分返回的 **uploadUrl** 属性是后续查询用于上载文件的字节范围的不透明 URL。 它包含 **expirationDateTime** 到期的后续`PUT`查询的适当身份验证令牌。 不自定义此 URL。
>
>**nextExpectedRanges** 属性指定要上载的下一个文件字节位置，例如， `"NextExpectedRanges":["2097152"]`。 必须按顺序上传文件中的字节。

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a>示例

### <a name="example-1-create-an-upload-session-to-add-a-large-attachment-to-a-draft-message"></a>示例 1：创建上载会话以将大附件添加到草稿邮件
以下示例演示如何创建可用于后续文件上载操作到指定邮件的上载会话。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession",
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/attachment-createuploadsession-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/attachment-createuploadsession-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/attachment-createuploadsession-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0uAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

### <a name="example-2-create-an-upload-session-to-add-a-large-in-line-attachment-to-a-draft-message"></a>示例 2：创建上载会话以将较大的内线附件添加到草稿邮件

以下示例演示如何创建上载会话，该会话可用于向草稿邮件添加大型内嵌附件。

对于内联附件，将 _isInline_ 属性 `true` 设置为 并使用 _contentId_ 属性指定附件的 CID，如下所示。 在草稿邮件正文中，使用相同的 CID 值指示要使用 CID HTML 引用标记包含附件的位置，例如 `<img src="cid:my_inline_picture">`。 成功上载文件后，呈现的邮件将在指定位置包含附件作为邮件正文的一部分。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession_inline",
  "sampleKeys": ["AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA="]
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "scenary", 
    "size": 7208534,
    "isInline": true,
    "contentId": "my_inline_picture"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-inline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-inline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-inline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/attachment-createuploadsession-inline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/attachment-createuploadsession-inline-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/attachment-createuploadsession-inline-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession_inline",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/gv1.0/users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/messages('AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA=')/AttachmentSessions('AAMkAGUwNjQ4ZjIxLTAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IjFTeXQ1bXdXYVh5UFJ",
    "expirationDateTime": "2021-12-27T14:20:12.9708933Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment: createUploadSession",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


