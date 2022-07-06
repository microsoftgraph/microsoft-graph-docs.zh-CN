---
title: 创建 taskFileAttachment
description: 将新的 taskFileAttachment 对象添加到 todoTask。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 590e8912178cdbc6eb0c2ed9f756ff2a77e84f9e
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645630"
---
# <a name="create-taskfileattachment"></a>创建 taskFileAttachment
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将新的 [taskFileAttachment](../resources/taskfileattachment.md) 对象添加 [到 todoTask](../resources/todotask.md)。

此操作限制可添加到 3 MB 以下的附件的大小。 如果文件附件的大小超过 3 MB，请 [创建上传会话](../api/taskfileattachment-createuploadsession.md) 以上传附件。


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
POST /me/todo/lists/{id}/tasks/{id}/attachments
POST /users/{id}/todo/lists/{id}/tasks/{id}/attachments
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [taskFileAttachment 对象的](../resources/taskfileattachment.md) JSON 表示形式。

创建文件附件时，包括 `"@odata.type": "#microsoft.graph.taskFileAttachment"` 所需属性。

|属性|类型|说明|
|:---|:---|:---|
|contentBytes|Binary|文件的 Base64 编码内容。 必需。|
|contentType|String|附件的内容类型。 |
|name|String|在表示嵌入附件的图标下显示的文本的名称。 这不必是实际的文件名。 必需。 |
|size|Int32|附件大小，以字节为单位。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [taskFileAttachment](../resources/taskfileattachment.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "create_taskFileAttachment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/AAMkpsDRVK=/tasks/AAKdfjhgsjhgJ=/attachments
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.taskFileAttachment",
  "name": "smile",
  "contentBytes": "a0b1c76de9f7=",
  "contentType": "image/gif"
}
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taskFileAttachment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.taskFileAttachment",
  "id": "AAMkADNkN2R",
  "lastModifiedDateTime": "2017-01-26T08:48:28Z",
  "name": "smile",
  "contentType": "image/gif",
  "size": 1008
}
```

