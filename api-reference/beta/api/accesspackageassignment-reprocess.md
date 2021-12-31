---
title: accessPackageAssignment：重新处理
description: 重新处理 accesspackageassignment 对象。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 66356cd856906ba73b107c06cfd36cc52bf85acb
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650865"
---
# <a name="accesspackageassignment-reprocess"></a>accessPackageAssignment：重新处理

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD中](../resources/entitlementmanagement-overview.md)，调用方可以自动重新计算和强制执行特定访问包的用户分配的[accessPackageAssignment](../resources/accesspackageassignment.md)对象。 访问 **包的 assignmentState** 必须供管理员重新处理 `Delivered` 用户的分配。 只有具有访问包分配管理器角色或更高权限的管理员Azure AD才能执行此操作。

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
POST /identityGovernance/entitlementManagement/accessPackageAssignments/{id}/reprocess 
```

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将返回 响应代码，并重新评估并强制用户分配 `202 Accepted` [accessPackageAssignment](../resources/accesspackageassignment.md) 对象，这意味着访问包的状态将更改为"已传递"。 如果工作分配不存在，此方法将返回 ，如果 `404 Not Found` **id** 无效，此方法将返回 响应 `400 Bad Request` 代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignments"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
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
