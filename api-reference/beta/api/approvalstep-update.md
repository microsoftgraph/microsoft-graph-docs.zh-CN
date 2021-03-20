---
title: 更新 approvalStep
description: 对 approvalStep 对象应用批准或拒绝决定。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b8ef436a9319e7a670e0aa5bdc728b39b53c2709
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942519"
---
# <a name="update-approvalstep"></a>更新 approvalStep

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对 approvalStep 对象应用 [批准或拒绝](../resources/approvalStep.md) 决定。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。 必填。 |

## <a name="request-body"></a>请求正文

下表显示了此方法所需的属性。

| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
| reviewResult | String | 审批者的决定。 可取值为：`Approve`、`Deny`。|
| justification | String | 与审批者的决定相关的理由。 |


## <a name="response"></a>响应

如果成功，此方法在响应 `204 No Content` 正文中返回 响应代码。 但是，如果调用方没有适当的权限，该方法将返回 响应代码，或者如果未找到审批 `403 Forbidden` ID，则该方法返回 `404 Not found` 。 如果请求已在同一审批阶段由另一个审批者批准，该方法在响应 `409 Conflict` 正文中返回。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_approvalstep"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-approvalstep-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
Content-Type: application/json
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patch approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
