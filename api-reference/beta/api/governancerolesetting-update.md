---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
ms.openlocfilehash: ca5752d51e5d59578594a12c80ae1cac316b48bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041717"
---
# <a name="update-governancerolesetting"></a>更新 governanceRoleSetting

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

更新的[governanceRoleSetting](../resources/governancerolesetting.md)属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | PrivilegedAccess.ReadWrite.AzureResources |

除了权限范围，此 API 要求至少有一个请求程序`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。
## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-request-headers"></a>可选的请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | 持有者 {code}|
| Content-type  | application/json|


## <a name="request-body"></a>请求正文
在请求正文中，提供[governanceRuleSettings](../resources/governancerulesetting.md)更新所需的值。 

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|管理员尝试添加合格的角色分配时计算规则设置。|
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|管理员尝试添加直接成员角色分配时计算规则设置。|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|当用户尝试添加合格的角色分配时计算规则设置。 此操作不受支持的`pimforazurerbac`方案现在，以及可在以后的方案。|
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|当用户尝试激活其角色分配时计算规则设置。|

## <a name="response"></a>响应
如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。 

## <a name="error-codes"></a>错误代码
此 API 遵循标准的 HTTP 代码。 此外，如下所示的自定义的错误代码。
|错误代码     | 错误消息         | 详细信息             |
|:--------------| :---------------------|:--------------------|
| 400 BadRequest| RoleSettingNotFound   | [GovernanceRoleSetting](../resources/governancerolesetting.md)系统中不存在。
| 400 BadRequest| InvalidRoleSetting    | 在请求正文中提供的[governanceRuleSettings](../resources/governancerulesetting.md)值不是有效的。

## <a name="example"></a>示例 
本示例更新自定义角色 3 中的订阅 Wingtip Toys-prod 移角色设置。
##### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
  "adminEligibleSettings":[{"ruleIdentifier":"ExpirationRule","setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"}]
}
```
##### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
