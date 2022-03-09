---
title: 更新 approvalStage
description: 对 approvalStage 对象应用批准或拒绝决定。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 62aafeda3d6f04ffd1f195ea8f1cdb9ac8d89891
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63398092"
---
# <a name="update-approvalstage"></a>更新 approvalStage

命名空间：microsoft.graph

在[Azure AD中，](../resources/entitlementmanagement-overview.md)批准或拒绝[审批中的 approvalStage](../resources/approvalstage.md) [对象](../resources/approval.md)。

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
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{accessPackageAssignmentRequestId}/stages/{approvalStageId}
```

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文

下表显示了此方法所需的属性。

| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
| reviewResult | String | 审批者的决定。 可取值为：`Approve`、`Deny`。 必需。|
| justification | String | 与审批者决策相关的理由。 |


## <a name="response"></a>响应

如果成功，此方法在响应 `204 No Content` 正文中返回 响应代码。 IOf 调用方没有正确的权限，该方法返回 响应 `403 Forbidden` 代码，或者如果未找到审批 ID，则该方法返回 `404 Not found`。 如果请求已在同一审批阶段由另一个审批者批准，该方法将返回 `409 Conflict` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "patch_approvalstage"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/stages/d4fa4045-4716-436d-aec5-57b0a713f095

{
 "reviewResult":"Approve",
 "justification":"OK"
}
```

### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patch approvalStage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
