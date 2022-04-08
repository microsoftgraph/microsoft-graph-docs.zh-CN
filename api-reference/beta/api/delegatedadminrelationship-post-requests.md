---
title: 创建请求
description: 创建新的 delegatedAdminRelationshipRequest 对象。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: df8e80f55e51c5b720e791243668fa468c1bcea6
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704394"
---
# <a name="create-requests"></a>创建请求
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| DelegatedAdminRelationship.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/requests
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) 对象的 JSON 表示形式。

创建 **delegatedAdminRelationshipRequest** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|action|delegatedAdminRelationshipRequestAction|要对委派的管理关系执行的操作。 必需。 可能的值为： `lockForApproval`. `terminate`|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) 对象。 响应包含一个 **Location** 标头，其中包含创建的委派管理员关系请求的 URL。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_delegatedadminrelationshiprequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/requests
Content-Type: application/json

{
  "action": "lockForApproval"
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Location: https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/c45e5ffb-3de2-4938-a214-b7eed802db66-4be56058-bb48-4a8e-8282-6cf0e98e6c9d/requests/5a6666c9-7282-0a41-67aa-25a5a3fbf339

{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipRequest",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#requests",
  "id": "5a6666c9-7282-0a41-67aa-25a5a3fbf339",
  "action": "lockForApproval",
  "status": "created",
  "createdDateTime": "2022-02-10T10:55:47.1180588Z",
  "lastModifiedDateTime": "2022-02-10T10:55:47.1180588Z"
}
```

