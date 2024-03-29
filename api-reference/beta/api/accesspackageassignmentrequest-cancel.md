---
title: accessPackageAssignmentRequest：cancel
description: 取消处于可取消状态的访问PackageAssignmentRequest 对象。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 36b14cd39b01ec95b248ad151f7e13f6deb9bed9
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650760"
---
# <a name="accesspackageassignmentrequest-cancel"></a>accessPackageAssignmentRequest：cancel
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

In [Azure AD Entitlement Management](../resources/entitlementmanagement-overview.md)， cancel [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects that are in a cancellable state： `accepted` ， ， ， `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|EntitlementManagement.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象的 JSON 表示形式。

对于取消自己的请求的非管理员用户，请求必须包含 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)的 **ID** 和值为 的 **requestStatus。** `cancelled`

## <a name="response"></a>响应

如果成功，此方法返回 `200 OK` 响应代码。  它不会在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel

{
  "id":"request-id",
  "requestStatus":"cancelled"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

