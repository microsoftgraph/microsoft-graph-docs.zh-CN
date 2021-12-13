---
title: 创建 taskList
description: 创建新的 taskList 对象。
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2403bf72748a202bf474487f144967a0f1590a7d
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424823"
---
# <a name="create-basetasklist"></a>创建 baseTaskList
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [taskList](../resources/basetasklist.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
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
POST /me/tasks/lists
POST /users/{userId|userPrincipalName}/tasks/lists
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [baseTaskList](../resources/basetasklist.md) 对象的 JSON 表示形式。

下表显示创建 **baseTaskList 时所需的属性**。

|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|指示任务列表标题的字段。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [baseTaskList](../resources/basetasklist.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_tasklist_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/tasks/lists
Content-Type: application/json

{
    "displayName": "Shopping list"
}
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taskList"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.taskList",
    "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAABCE3Uw==\"",
    "displayName": "Shopping list",
    "id": "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNi"
}
```

