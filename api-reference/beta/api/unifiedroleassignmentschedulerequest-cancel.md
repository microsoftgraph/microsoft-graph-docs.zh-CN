---
title: unifiedRoleAssignmentScheduleRequest：cancel
description: 取消 unifiedRoleAssignmentScheduleRequest。
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4770603d5b0cc57830f089a42351608a0c75bbca
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453770"
---
# <a name="unifiedroleassignmentschedulerequest-cancel"></a>unifiedRoleAssignmentScheduleRequest：cancel
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

立即取消 [处于状态的 unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象，并请系统在 30 天后自动删除已取消 `Granted` 的请求。 调用此操作后， **已** 取消的 unifiedRoleAssignmentScheduleRequest 的状态将改为 `Canceled` 。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleAssignmentSchedule.ReadWrite.Directory、RoleManagement.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|不支持|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。 尝试取消处于不可取消状态的请求，例如，状态为 或 的 unifiedRoleAssignmentScheduleRequest 对象 `Provisioned` `Failed` 将返回 `400 Bad Request` 错误代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/15fec3d4-64b1-4b03-beb7-f1ba6dddf6cc/cancel
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleassignmentschedulerequest-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleassignmentschedulerequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleassignmentschedulerequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleassignmentschedulerequest-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

