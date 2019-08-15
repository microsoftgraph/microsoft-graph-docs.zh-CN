---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 6cbcdfbd3406226e23000c472467a42604c16c90
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419669"
---
# <a name="update-governancerolesetting"></a>更新 governanceRoleSetting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新[governanceRoleSetting](../resources/governancerolesetting.md)的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

>**注意:** 此 API 还要求请求者在资源上至少有`Active`一个管理员角色分配`owner` ( `user access administrator`或)。

|权限类型      | 权限              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess AzureResources  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|


## <a name="request-body"></a>请求正文
在请求正文中, 提供需要更新的[governanceRuleSettings](../resources/governancerulesetting.md)的值。 

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)集合|在管理员尝试添加符合条件的角色分配时评估的规则设置。|
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md)集合|在管理员尝试添加直接成员角色分配时评估的规则设置。|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)集合|用户尝试添加符合条件的角色分配时评估的规则设置。 目前不支持这`pimforazurerbac`种情况, 在将来的方案中可能会用到。|
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md)集合|用户尝试激活他的角色分配时评估的规则设置。|

## <a name="response"></a>响应
如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。 

### <a name="error-codes"></a>错误代码
此 API 返回标准的 HTTP 错误代码。 此外, 它还返回以下自定义错误代码。

|错误代码     | 错误消息         | 详细信息             |
|:--------------| :---------------------|:--------------------|
| 400 BadRequest| RoleSettingNotFound   | [GovernanceRoleSetting](../resources/governancerolesetting.md)在系统中不存在。
| 400 BadRequest| InvalidRoleSetting    | 请求正文中提供的[governanceRuleSettings](../resources/governancerulesetting.md)值无效。

## <a name="example"></a>示例 
本示例更新订阅 Wingtip 玩具-生产版中的自定义角色3的角色设置。
##### <a name="request"></a>请求

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
   "adminEligibleSettings":[
      {
         "ruleIdentifier":"ExpirationRule",
         "setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
      }
   ]
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

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
