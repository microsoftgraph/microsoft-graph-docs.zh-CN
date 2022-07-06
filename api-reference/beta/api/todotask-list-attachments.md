---
title: 列出 taskFileAttachments
description: 获取 taskFileAttachment 对象及其属性的列表。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 66caaea5cf604ab85cd7e64c4a4ca088c2db2b6f
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645636"
---
# <a name="list-taskfileattachments"></a>列出 taskFileAttachments
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [taskFileAttachment](../resources/taskfileattachment.md) 对象及其属性的列表。 不会在响应中返回 **contentBytes** 属性。 使用 [Get 附件](../api/attachment-get.md) API 查看 **内容字节**。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.Read、Tasks.ReadWrite|
|委派（个人 Microsoft 帐户）|Tasks.Read、Tasks.ReadWrite|
|Application|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/attachments
GET /users/{id}/todo/lists/{id}/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [taskFileAttachment](../resources/taskfileattachment.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "list_taskfileattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMehdkfuhgAAA=/tasks/AAMkAGUzY5QKjAAA=/attachments
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taskFileAttachment",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.taskFileAttachment",
            "id": "AAMkADliMm=",
            "name": "flower.md",
            "size": 2814,
            "lastModifiedDateTime": "2022-06-09T10:40:52Z",
            "contentType": "application/octet-stream"
        },
        {
            "@odata.type": "#microsoft.graph.taskFileAttachment",
            "id": "AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwBGAAAAAADdOMUbUmCfTKa7OC-fqjkdBwBnu3olF7NfToRyJ2f__TNcAAAAAAESAABnu3olF7NfToRyJ2f__TNcAAHmG2K0AAABEgAQAFWmGvX71MhOrjRDhWM95yY=",
            "name": "tree.jpg",
            "size": 8591,
            "lastModifiedDateTime": "2022-06-09T10:40:59Z",
            "contentType": "image/jpeg"
        }
    ]
}
```
