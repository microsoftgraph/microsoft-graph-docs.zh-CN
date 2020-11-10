---
title: 更新 authorizationpolicy
description: 更新 authorizationPolicy 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd6d618c7aab7e3e9f3c4339ce840c6b2dc0a1f6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961442"
---
# <a name="update-authorizationpolicy"></a>更新 authorizationPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [authorizationPolicy](../resources/authorizationpolicy.md) 对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Policy.ReadWrite.Authorization|
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | Policy.ReadWrite.Authorization|

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | 持有者 {token} |
| Content-type | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|  
|displayName|String| 此策略的显示名称。 |  
|说明|String| 此策略的说明。 |  
|guestUserRoleId|Guid| 表示应向来宾用户授予的角色的角色 templateId。 若要查找可用角色模板的列表，请参阅 [List unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) 。 目前只有受支持的角色是用户 (a0b1b346-4d3e-4e8b-98f8-753987be4970) 、来宾用户 (10dae51f-b6af-4016-8d66-8c2a99b929b3) 和受限制的来宾用户 (2af84b1e-32c8-42b7-82bc-daa82404023b) 。 | 
|enabledPreviewFeatures|集合 (字符串) | 租户上启用了专用预览的功能列表。 | 
|blockMsolPowerShell|Boolean| 若要禁用 MSOL PowerShell 的使用，请将此属性设置为 `true` 。 设置为 `true` 将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。 这不会影响 Azure AD Connect 或 Microsoft Graph。 | 
|defaultUserRolePermissions|[defaultUserRolePermissions](../resources/defaultUserRolePermissions.md)| 指定默认用户角色的某些可自定义权限。 | 
|allowedToUseSSPR|Boolean| 指示租户上的用户是否可以使用 Self-Serve 密码重置功能。 | 
|allowedToSignUpEmailBasedSubscriptions|Boolean| 指示用户是否可以注册基于电子邮件的订阅。 | 
|allowEmailVerifiedUsersToJoinOrganization|Boolean| 指示用户是否可以通过电子邮件验证加入租户。 |
| permissionGrantPolicyIdsAssignedToDefaultUserRole | String collection | 指示是否允许用户同意应用程序，如果是，则使用哪个 [应用程序同意策略](/azure/active-directory/manage-apps/manage-app-consent-policies) 来控制授予许可的用户的权限。 值的格式应为 `managePermissionGrantsForSelf.{id}` ，其中 `{id}` 是内置或自定义 [应用程序许可策略](/azure/active-directory/manage-apps/manage-app-consent-policies)的 **id** 。 空列表指示用户同意应用程序已被禁用。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a>示例1：更新或设置租户的来宾用户访问级别

#### <a name="request"></a>请求

下面展示了示例请求。 在此示例中，将来宾访问级别修改为受限制的来宾用户。

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "guestUserRole":"2af84b1e-32c8-42b7-82bc-daa82404023b"
}
```

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a>示例2：在租户上为预览启用新功能

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_preview"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "enabledPreviewFeatures":[
      "assignGroupsToRoles"
   ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-preview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-preview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-preview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-preview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-block-msol-powershell-in-tenant"></a>示例3：阻止租户中的 MSOL PowerShell

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "blockMsolPowerShell":true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-blockmsolpowershell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a>示例4：禁用默认用户角色的权限以创建应用程序

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "defaultUserRolePermissions":{
      "allowedToCreateApps":false
   }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a>示例5：启用默认用户角色以使用 Self-Serve 密码重置功能

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "allowedToUseSSPR":true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-sspr-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-disable-user-consent-to-apps-for-default-user-role"></a>示例6：禁止用户同意默认用户角色的应用程序

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "permissionGrantPolicyIdsAssignedToDefaultUserRole":[
   
   ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-disableuserconsent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-disableuserconsent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-disableuserconsent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-disableuserconsent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-7-enable-user-consent-to-apps-subject-to-app-consent-policy"></a>示例7：允许用户同意应用程序，受应用程序许可策略的制约 

#### <a name="request"></a>请求

以下是允许用户同意应用程序的请求的示例，具体取决于内置 [应用程序许可策略，该策略](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low` 允许委派权限归为 "低"，适用于来自已验证的发布者或在同一租户中注册的客户端应用程序。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "permissionGrantPolicyIdsAssignedToDefaultUserRole":[
      "managePermissionGrantsForSelf.microsoft-user-default-low"
   ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-enableuserconsentlow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-enableuserconsentlow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-enableuserconsentlow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-enableuserconsentlow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
