---
title: accessPackageAssignmentRequest：重新处理
description: 重新处理 accessPackageAssignmentRequest 对象。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 39104bb29ba7b1f8a9e672775781a5303ab0fa81
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650739"
---
# <a name="accesspackageassignmentrequest-reprocess"></a>accessPackageAssignmentRequest：重新处理

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD中](../resources/entitlementmanagement-overview.md)，调用方可以自动重试用户访问访问包的请求。 在 **requestState** 处于 或 状态的 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象 `DeliveryFailed` 上 `PartiallyDelivered` 执行。 

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户） | EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | EntitlementManagement.ReadWrite.All |
  
## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentsRequests/{id}/reprocess  
```

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将返回  `202 Accepted` 响应代码并重试请求。 如果[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象不存在，此方法将返回 ，如果 id 无效， `404 Not Found` 此方法将返回 `400 Bad Request` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignmentsrequest"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
```

### <a name="response"></a>响应

下面展示了示例响应。


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted  
```
