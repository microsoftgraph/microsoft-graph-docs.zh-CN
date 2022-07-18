---
title: 更新 unifiedRoleManagementPolicyRule
description: 更新为角色管理策略定义的规则。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9007f0e5907c5a2906f8bb3e2efe59f0b7704ab9
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900378"
---
# <a name="update-unifiedrolemanagementpolicyrule"></a>更新 unifiedRoleManagementPolicyRule
命名空间：microsoft.graph

更新为角色管理策略定义的规则。 该规则可以是从 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象派生的以下类型之一：
+ [unifiedRoleManagementPolicyApprovalRule](../resources/unifiedrolemanagementpolicyapprovalrule.md)
+ [unifiedRoleManagementPolicyAuthenticationContextRule](../resources/unifiedrolemanagementpolicyauthenticationcontextrule.md)
+ [unifiedRoleManagementPolicyEnablementRule](../resources/unifiedrolemanagementpolicyenablementrule.md)
+ [unifiedRoleManagementPolicyExpirationRule](../resources/unifiedrolemanagementpolicyexpirationrule.md)
+ [unifiedRoleManagementPolicyNotificationRule](../resources/unifiedrolemanagementpolicynotificationrule.md)

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleManagementPolicy.ReadWrite.Directory、RoleManagement.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|claimValue|String|身份验证上下文声明的值。 <br/><br/>可以针对 **unifiedRoleManagementPolicyAuthenticationContextRule** 规则类型进行更新。|
|enabledRules|字符串集合|为此策略规则启用的规则的集合。 例如，`MultiFactorAuthentication``Ticketing`和 `Justification`.<br/><br/>可以针对 **unifiedRoleManagementPolicyEnablementRule** 规则类型进行更新。|
|isDefaultRecipientsEnabled|Boolean|指示默认收件人是否会收到通知电子邮件。<br/><br/>可以针对 **unifiedRoleManagementPolicyNotificationRule** 规则类型进行更新。|
|isEnabled|Boolean| 是否启用此规则。 <br/><br/>可以针对 **unifiedRoleManagementPolicyAuthenticationContextRule** 规则类型进行更新。|
|isExpirationRequired|Boolean|指示是否需要过期，或者它是永久活动分配还是资格。 <br/><br/>可以针对 **unifiedRoleManagementPolicyExpirationRule** 规则类型进行更新。|
|maximumDuration|期限| 资格或分配所允许的最长持续时间不是永久性的。 如果 **isExpirationRequired** 为 .，则 `true`为必需。 <br/><br/>可以针对 **unifiedRoleManagementPolicyExpirationRule** 规则类型进行更新。 |
|notificationLevel|String|通知级别。 可能的值是 `None`， `Critical`. `All`<br/><br/>可以针对 **unifiedRoleManagementPolicyNotificationRule** 规则类型进行更新。|
|notificationRecipients|字符串集合|电子邮件通知的收件人列表。<br/><br/>可以针对 **unifiedRoleManagementPolicyNotificationRule** 规则类型进行更新。|
|notificationType|String|通知的类型。 仅 `Email` 支持。<br/><br/>可以针对 **unifiedRoleManagementPolicyNotificationRule** 规则类型进行更新。|
|recipientType|String|通知的收件人的类型。 可能的值是 `Requestor`， `Approver`. `Admin`<br/>可以针对 **unifiedRoleManagementPolicyNotificationRule** 规则类型进行更新。|
|setting|[approvalSettings](../resources/approvalsettings.md)|用于批准角色分配的设置。 <br/><br/>可以针对 **unifiedRoleManagementPolicyApprovalRule** 规则类型进行更新。|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|定义角色管理策略规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。 <br/><br/> 可以针对所有规则类型进行更新。|

>**注意：**`@odata.type`具有特定规则类型的值的属性必须包含在正文中。 例如，`"@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule"`。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

以下示例使用 ID `Expiration_EndUser_Assignment`更新角色管理策略规则。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedrolemanagementpolicyrule"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/roleManagementPolicies/DirectoryRole_84841066-274d-4ec0-a5c1-276be684bdd3_200ec19a-09e7-4e7a-9515-cf1ee64b96f9/rules/Expiration_EndUser_Assignment
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
    "id": "Expiration_EndUser_Assignment",
    "isExpirationRequired": true,
    "maximumDuration": "PT1H45M",
    "target": {
        "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
        "caller": "EndUser",
        "operations": [
            "All"
        ],
        "level": "Assignment",
        "inheritableSettings": [],
        "enforcedSettings": []
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-unifiedrolemanagementpolicyrule-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-unifiedrolemanagementpolicyrule-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content

```
<!--
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```
-->
