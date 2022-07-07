---
title: 将文件附加到待办事项任务
description: 了解如何将大型文件附加到 Microsoft 待办任务，以及如何选择正确的方法将文件附加到任务。
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 2d4c66a6e6e2438f1d7b7aafc6555ab701d1883a
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671358"
---
# <a name="attach-files-to-a-to-do-task"></a>将文件附加到待办事项任务

使用 Microsoft Graph 中的待办事项 API，可将高达 25 MB 的文件附加到 [todoTask](/graph/api/resources/todotask)。 根据文件大小，选择以下两种方法之一来附加文件：
- 若要附加任何大小的文件，请创建上传会话，并迭代使用 `PUT` 上传文件的字节范围，直到上传整个文件为止。 最后一个成功 `PUT` 响应中的标头包括带附件 ID 的 URL。
- 如果文件大小小于 3 MB，请对 **todoTask****的附件** 导航属性执行单个`POST`；了解如何 [为任务](/graph/api/todotask-post-attachments)执行此操作。 成功的 `POST` 响应包括文件附件的 ID。

本文演示了第一种方法。 你将逐步了解如何创建和使用上传会话向任务添加文件附件。
## <a name="step-1-create-an-upload-session"></a>第 1 步：创建上传会话

[创建上传会话](/graph/api/taskfileattachment-createuploadsession) 以将文件附加到 **todoTask**。 在输入参数 [attachmentInfo 中](/graph/api/resources/attachmentinfo)指定文件。

成功的操作返回 `HTTP 201 Created` 和新的 [uploadSession](/graph/api/resources/uploadsession) 实例，其中包含可在后续 `PUT` 操作中用于上传文件各部分的非跳转 URL。 **uploadSession** 提供一个临时存储位置，在此位置保存文件字节数，直到完整文件上传完毕。

响应中的 **uploadSession** 对象还包括 **nextExpectedRanges** 属性，该属性指示初始上传起始位置应为字节 `0`。

### <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.ReadWrite|
|委派（个人 Microsoft 帐户）|Tasks.ReadWrite|
|Application|不支持。|

### <a name="example-create-an-upload-session-for-a-todotask"></a>示例：为 todoTask 创建上传会话

#### <a name="request"></a>请求

下面是创建上传会话的请求示例。
<!-- {
  "blockType": "request",
  "name": "todo_attachment_walkthrough_createuploadsession"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachments/createUploadSession
Content-Type: application/json

{
  "attachmentInfo": {
    "@odata.type": "microsoft.graph.attachmentInfo",
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```

#### <a name="response"></a>响应
以下示例显示响应正文中为任务返回的 **uploadSession** 资源。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=",
    "expirationDateTime": "2022-06-09T10:45:27.4324526Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a>步骤 2：使用上传会话上传文件的字节范围

如果要上传文件或文件的一部分，在 **uploadSession** 资源 **uploadUrl** 属性中，对第 1 步返回的 URL 进行 `PUT` 请求。 可上传整个文件，或将文件拆分为多个字节范围。 每个字节范围需要小于 4 MB。

指定请求标头和请求正文，如以下部分所述。

### <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
|Authorization | String | Bearer {token}。必需。 |
| Content-Length | Int32 | 此操作中上传的字节数。 每个 `PUT` 操作的字节数上限为 4 MB。 任何大于 4 MB 的请求都将失败。 必填。 |
| Content-Range | 字符串 | 在此操作中上传文件的基于 0 的字节范围，用格式 `bytes {start}-{end}/{total}` 表示。必填。 |
| Content-Type | String  | MIME 类型。 指定 `application/octet-stream`。 必填。 |


### <a name="request-body"></a>请求正文

指定要附加的文件的实际字节数，它们位于由 `Content-Range` 请求标头指定的位置范围内。

### <a name="response"></a>响应
成功上传将返回 `HTTP 200 OK` 响应代码和 **uploadSession** 对象。 请注意响应对象中的以下项：

-  **expirationDateTime** 属性值与步骤 1 中的初始 **uploadSession** 返回的值相同。
- **nextExpectedRanges** 指定上传开始的下一个字节位置，例如 `"nextExpectedRanges":["2097152"]`。 必须按顺序上传文件中的字节。
<!-- The **nextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"nextExpectedRanges":["2097152"]`.
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"nextExpectedRanges":["1998457-2097094"]`.
-->
- **uploadUrl** 属性不会显式返回，因为上传会话的所有 `PUT` 操作使用创建会话时返回的同一 URL（步骤 1）。

### <a name="example-first-upload-to-the-todotask"></a>示例：首先上传到 todoTask

#### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=/content
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>响应

下列示例响应在 **nextExpectedRanges** 属性中显示服务器预期的下一字节范围的起点。
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ExpirationDateTime":"2022-06-09T10:45:27.4324526Z",
  "NextExpectedRanges":["2097152"]
}
```

## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a>步骤 3：继续上传字节范围，直至完整文件上传完毕

执行步骤 2 中的初始上传后，在会话的到期日期/时间前，使用步骤 2 中所述的 `PUT` 请求，继续上传文件中剩余的部分。 使用 **nextExpectedRanges** 集合确定要上传的下一个字节范围的开头。 可能会发现指定的多个范围，这些范围指明了服务器尚未收到的文件部分。 如果需要恢复中断的传输，并且客户端不能确定服务的状态，这个方法很有用。

成功上传文件的最后一个字节后，最终 `PUT` 操作将返回 `HTTP 201 Created` 响应代码和指示文件附件 URL 的 `Location` 标头。 可从 URL 获取附件 ID 并将其保存供以后使用。

下列示例显示在此处理步骤中将文件的最后一个字节范围上传到 **todoTask** 。

### <a name="example-final-upload-to-the-todotask"></a>示例：最终上传到 todoTask

#### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=/content
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

Location: https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/Attachments/AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=
Content-Length: 0
```

## <a name="alternative-step-cancel-the-upload-session"></a>替代步骤：取消上传会话
在上传会话到期之前的任何时间，如果必须取消上传，可使用同一初始非跳转 URL 来删除上传会话。 成功的操作返回 `204 No Content` 响应代码。

### <a name="example-cancel-the-upload-session"></a>示例：取消上传会话

#### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=
```

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```

