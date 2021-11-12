---
title: 创建 linkedResource
description: 创建新的 linkedResource 对象。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 931ed73c65cc328075049c240309f4d7c3188222
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60943617"
---
# <a name="create-linkedresource"></a>创建 linkedResource
命名空间：microsoft.graph

创建 [linkedResource](../resources/linkedresource.md) 对象以将指定 [任务](../resources/todotask.md) 与合作伙伴应用程序中的项目关联。 例如，可以将任务与任务中Outlook项关联，并可以创建 **linkedResource** 对象来跟踪其关联。

还可以在创建任务 时创建 **linkedResource** [对象](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples)。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
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
|id|String|链接实体的服务器生成的 ID 继承自 [实体](../resources/entity.md)|
|WebUrl|String|链接到链接实体的深层链接 |
|applicationName|String|指示发送链接实体的源的应用程序名称的字段 |
|displayName|String|指示链接实体的标题的字段。 |
|externalId|String|第三方/合作伙伴系统上与此任务关联的对象的 ID |



## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [linkedResource](../resources/linkedresource.md) 对象。

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
POST https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
Content-Type: application/json

{
  "webUrl": "https://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-linkedresource-from-linkedresources-java-snippets.md)]
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



