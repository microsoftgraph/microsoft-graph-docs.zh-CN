---
title: 删除 checklistItem
description: 删除 checklistItem 对象。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5c308d9c58c11400529c3f1b938a6f70f7d4ffd
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821315"
---
# <a name="delete-checklistitem"></a>删除 checklistItem
命名空间：microsoft.graph

删除 [checklistItem](../resources/checklistitem.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.ReadWrite|
|委派（个人 Microsoft 帐户）|Tasks.ReadWrite|
|应用程序|Tasks.ReadWrite|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems/{checklistItemId}
DELETE /users/{id | userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems/{checklistItemId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "delete_checklistitem"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/checklistitems/e3a26c2e-7c6f-4317-9d71-c27267008202
```

### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

