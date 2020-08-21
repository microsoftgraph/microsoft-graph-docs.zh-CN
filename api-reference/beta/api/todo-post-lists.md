---
title: 创建 todoTaskList
description: 创建新的列表对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2628721edff8ad1dad559e590c3dade972220c73
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849899"
---
# <a name="create-todotasklist"></a>创建 todoTaskList
命名空间：microsoft.graph

创建新的列表对象。

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
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
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
|displayName|String|指示任务列表标题的域。|

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回响应代码和 [todoTaskList](../resources/todotasklist.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_todotasklist_from_lists"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists
Content-Type: application/json
Content-length: 60

{
  "displayName": "Travel items",
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
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "AAMkADIyAAAhrbPWAAA=",
  "displayName": "Travel items",
  "isOwner": true,
  "isShared": false,
  "wellknownListName": "none"
}
```