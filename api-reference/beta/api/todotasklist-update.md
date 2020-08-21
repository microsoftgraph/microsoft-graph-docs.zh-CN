---
title: 更新 todoTaskList
description: 更新 todoTaskList 对象的属性。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bedcf564fdc470a6bfcf1dacafe2efa82694e0ed
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849875"
---
# <a name="update-todotasklist"></a>更新 todoTaskList
命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [todoTaskList 对象的](../resources/todotasklist.md) 属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.ReadWrite|
|委派（个人 Microsoft 帐户）|Tasks.ReadWrite|
|应用|不支持|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [todoTaskList](../resources/todotasklist.md) 对象的 JSON 表示形式。

下表显示创建 [todoTaskList 时所需的属性](../resources/todotasklist.md)。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|指示任务列表的更新标题的域。|



## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [更新的 todoTaskList](../resources/todotasklist.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPWAAA="],
  "name": "update_todotasklist"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAhrbPWAAA=
Content-Type: application/json
Content-length: 167

{
  "displayName": "Vacation Plan",
}
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTaskList"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "AAMkADIyAAAhrbPWAAA=",
  "displayName": "Vacation Plan",
  "isOwner": true,
  "isShared": false,
  "wellknownListName": "none"
}
```

