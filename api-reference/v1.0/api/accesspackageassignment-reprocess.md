---
title: accessPackageAssignment：重新处理
description: 重新处理 accesspackageassignment 对象。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 75d221efa4c740eadb132ef429ac5d193512f3c6
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698528"
---
# <a name="accesspackageassignment-reprocess"></a>accessPackageAssignment：重新处理

命名空间：microsoft.graph

在 [Azure AD 权利管理](../resources/entitlementmanagement-overview.md)中，调用方可以自动重新评估和强制执行特定访问包用户分配的 [accessPackageAssignment](../resources/accesspackageassignment.md) 对象。 访问包的 **assignmentState** 必须 `Delivered` 供管理员重新处理用户的分配。 只有具有访问包分配管理器角色或更高版本的管理员才能在 Azure AD 权利管理中执行此操作。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户） | EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用 | EntitlementManagement.ReadWrite.All |
  
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
| Authorization | 持有者 \{token\}。 必填。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将返回 `202 Accepted` 响应代码并重新评估并强制用户分配 [accessPackageAssignment](../resources/accesspackageassignment.md) 对象，这意味着访问包的状态将更改为“已交付”。 如果分配不存在，则此方法将返回 `404 Not Found` ，或者如果 **ID** 无效，则此方法将返回 `400 Bad Request` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignments"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignments/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
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