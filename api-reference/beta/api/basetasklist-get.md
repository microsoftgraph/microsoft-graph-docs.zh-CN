---
title: 获取 baseTaskList
description: 读取 baseTaskList 对象的属性和关系。
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ba3922a6d1b36f8ef5181a81d3e82973b3d20677
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424830"
---
# <a name="get-basetasklist"></a>获取 baseTaskList
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [baseTaskList 对象的属性和](../resources/basetasklist.md) 关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.Read|
|委派（个人 Microsoft 帐户）|Tasks.Read|
|应用|不支持|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/tasks/lists/{baseTaskListId}
GET /users/{userId|userPrincipalName}/tasks/lists/{baseTaskListId}
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

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [baseTaskList](../resources/basetasklist.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_basetasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/tasks/lists/AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAADG6BbDxY
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.baseTaskList"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('43e9e4fb-be9f-4ee4-b879-59688955ed54')/tasks/lists/$entity",
    "@odata.type": "#microsoft.graph.wellKnownTaskList",
    "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAAAAAAkw==\"",
    "wellKnownListName": "defaultList",
    "displayName": "Tasks",
    "id": "AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAADG6BbDxY"
}
```

