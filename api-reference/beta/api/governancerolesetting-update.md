---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 96ddd9c1da7676ec3a61e2178ada6b973a9c760d
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398365"
---
# <a name="update-governancerolesetting"></a>更新 governanceRoleSetting

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

更新 [governanceRoleSetting](../resources/governancerolesetting.md) 的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。

>**注意：** 此 API 还要求请求者至少有一个 `Active` 管理员角色分配 (`owner` 或 `user access administrator`) 资源。

|权限类型      | 权限              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |
### <a name="azure-resources"></a>Azure 资源

| 权限类型 | 权限 |
|:--------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | 不支持。 |

### <a name="azure-ad"></a>Azure AD

| 权限类型 | 权限 |
|:--------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureAD |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | 不支持。 |

### <a name="groups"></a>组

|权限类型 | 权限 |
|:-------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureADGroup |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | 持有者 {token}|
| Content-type  | application/json|


## <a name="request-body"></a>请求正文
在请求正文中，提供需要更新的 [governanceRuleSettings 的](../resources/governancerulesetting.md) 值。 

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) 集合|管理员尝试添加符合条件的角色分配时评估的规则设置。|
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) 集合|管理员尝试添加直接成员角色分配时评估的规则设置。|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) 集合|当用户尝试添加符合条件的角色分配时评估的规则设置。 |
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) 集合|当用户尝试激活其角色分配时评估的规则设置。|

## <a name="response"></a>响应
如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。 

### <a name="error-codes"></a>错误代码
此 API 返回标准 HTTP 错误代码。 此外，它返回以下自定义错误代码。

|错误代码     | 错误消息         | 详细信息             |
|:--------------| :---------------------|:--------------------|
| 400 BadRequest| RoleSettingNotFound   | [governanceRoleSetting](../resources/governancerolesetting.md) 在系统中不存在。
| 400 BadRequest| InvalidRoleSetting    | 请求正文中提供的 [governanceRuleSettings](../resources/governancerulesetting.md) 值无效。

## <a name="example"></a>示例 
本示例更新订阅 Wingtip Toys - Prod 中自定义角色 3 的角色设置。
##### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json

{
   "adminEligibleSettings":[
      {
         "ruleIdentifier":"ExpirationRule",
         "setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
      }
   ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-governancerolesetting-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-governancerolesetting-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


