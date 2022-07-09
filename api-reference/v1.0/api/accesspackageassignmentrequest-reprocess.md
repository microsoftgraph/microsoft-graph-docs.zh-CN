---
title: accessPackageAssignmentRequest：重新处理
description: 重新处理 accessPackageAssignmentRequest 对象。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0ec27bd2dc451f95b3c001188924fa8c0077211b
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698519"
---
# <a name="accesspackageassignmentrequest-reprocess"></a>accessPackageAssignmentRequest：重新处理

命名空间：microsoft.graph

在 [Azure AD 权利管理](../resources/entitlementmanagement-overview.md)中，调用方可以自动重试用户对访问包的访问请求。 它对 **requestState** `DeliveryFailed` 处于或`PartiallyDelivered`状态的 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象执行。 

只能在完成原始请求后的 14 天内重新处理请求。 对于已完成超过 14 天的请求，需要要求用户取消请求 () 并在 [MyAccess](https://myaccess.microsoft.com/) 门户中发出新请求。

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
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/reprocess
```

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。 必填。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将返回  `202 Accepted` 响应代码并重试请求。 如果 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象不存在，则此方法将返回 `404 Not Found` ，或者如果 **ID** 无效，此方法将返回 `400 Bad Request` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "ignored",
  "name": "reprocess_accesspackageassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/d82eb508-acc4-43cc-bcf1-7c1c4a2c073b/reprocess
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
