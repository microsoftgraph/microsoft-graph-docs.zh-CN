---
title: 创建 linkedResources
description: 创建新的 linkedResources 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4311af292480a51eeaaefabb1ef8cf277b211e2c
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873243"
---
# <a name="create-linkedresources"></a>创建 linkedResources
命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 linkedResources 对象。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.ReadWrite|
|委派（个人 Microsoft 帐户）|Tasks.ReadWrite|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [linkedResource](../resources/linkedresource.md) 对象的 JSON 表示形式。

下表显示创建 [linkedResource](../resources/linkedresource.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|从[实体](../resources/entity.md)继承的链接实体的服务器生成 Id|
|webUrl|String|Deeplink 到链接实体 |
|applicationName|String|指示发送链接实体的源的应用程序名称的字段 |
|displayName|String|指示链接实体的标题的字段。 |
|externalId|String|与第三方/合作伙伴系统上的此任务相关联的对象的 Id |



## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [linkedResource](../resources/linkedresource.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "create_linkedresource_from_linkedresources"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```

