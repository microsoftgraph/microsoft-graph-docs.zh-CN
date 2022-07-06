---
title: taskFileAttachment：createUploadSession
description: 创建上传会话，以迭代方式将文件范围作为附件上传到 Microsoft To Do 任务。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a6a8aec00fcca1bbc50b25791c06db73cdd747f8
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645640"
---
# <a name="taskfileattachment-createuploadsession"></a>taskFileAttachment：createUploadSession
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建上传会话，以迭代方式将文件范围作为附件上传到 [todoTask](../resources/todotask.md)。

作为响应的一部分，此操作返回可在后续顺序 `PUT` 查询中使用的上传 URL。 通过每个 `PUT` 操作的请求标头，可以指定要上传的字节的确切范围。 这允许在上传期间删除网络连接的情况下恢复传输。

下面是使用上传会话将文件附加到 Microsoft To Do 任务的步骤：

1. 创建上传会话。
2. 在该上传会话中，每次) 时，以迭代方式上传字节范围 (高达 4 MB，直到上传文件的所有字节，并将文件附加到 **todoTask**。
3. 可选：删除上传会话。

>**注意：** 使用此方法可附加任何支持大小在 0 MB 到 25 MB 之间的文件。

有关描述端到端附件过程的示例，请参阅 [将文件附加到“执行”任务](/graph/todo-attachments)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.ReadWrite|
|委派（个人 Microsoft 帐户）|Tasks.ReadWrite|
|Application|不支持。|


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{id}/tasks/{id}/attachments/createUploadSession
POST /users/{id}/todo/lists/{id}/tasks/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|attachmentInfo|[attachmentInfo](../resources/attachmentinfo.md)|表示要上传和附加的项的属性。 至少指定附件类型 () `file` 、名称和文件大小。|


## <a name="response"></a>响应

如果成功，此操作将在响应正文中返回 `200 OK` 响应代码和新的 [uploadSession](../resources/uploadsession.md) 。

## <a name="examples"></a>示例

### <a name="request"></a>请求
下面是创建上传会话的请求示例。
<!-- {
  "blockType": "request",
  "name": "attachmentbasethis.createuploadsession"
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

### <a name="response"></a>响应
下面展示了示例响应。
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