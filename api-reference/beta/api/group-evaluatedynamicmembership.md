---
title: group：evaluateDynamicMembership
description: 评估用户或设备是否为或将成为动态组的成员。
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 778ed1164d41d05193dae32f90187ab6f3d4604a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208734"
---
# <a name="group-evaluatedynamicmembership"></a>group：evaluateDynamicMembership

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

评估用户或设备是否为动态组的成员。 会返回成员资格规则以及评估中使用的其他详细信息。 可以通过以下方式完成此操作：

- 评估用户或设备是否是指定动态组的成员。
- 根据用户或设备的 ID 和成员身份规则评估用户或设备是否是动态组的成员。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a>使用成员 ID 和组 ID 评估动态成员身份

| 权限类型                        | 权限（从最低特权到最高特权）                                                                                          |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | 对于用户：Group.Read.All 和 User.Read.All、Directory.Read.All<br>对于设备：Group.Read.All 和 Device.Read.All、Directory.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                                                                                                       |
| Application                            | 不支持。                                                                                                                       |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a>使用成员 ID 和成员身份规则评估动态成员身份

| 权限类型                        | 权限（从最低特权到最高特权）                                                    |
| :------------------------------------- | :--------------------------------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | 对于用户：User.Read.All、Directory.Read.All<br>对于设备：Device.Read.All、Directory.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                                                                 |
| Application                            | 不支持。                                                                                 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明      |
| :------------ | :--------------- |
| Authorization | 持有者 {token}   |
| Content-type  | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供所需的属性。

下表列出了评估组成员身份时所需的属性。

| 参数      | 类型              | 说明                                                                                                                                                                                                                                                                                                                                                                                                            |
| :------------- | :---------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| memberId       | 字符串集合 | memberId 是要评估的用户或设备的对象 ID。                                                                                                                                                                                                                                                                                                                                                       |
| membershipRule | 字符串集合 | 用于成员资格评估的规则。 如果未提供此属性，则会评估现有组的规则。 如果提供了此属性，则会评估用户或设备是否可以加入具有相同规则的组。 有关详细信息，请参阅 [Azure Active Directory 中的组动态成员资格规则](/azure/active-directory/users-groups-roles/groups-dynamic-membership)。 |

## <a name="response"></a>响应

如果成功，此方法将返回 `200 OK` 响应代码和 [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a>示例 1：评估用户或设备是否是现有组的成员

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_1"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/evaluateDynamicMembership
Content-type: application/json

{
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-1-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-1-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-1-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-1-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-evaluatedynamicmembership-1-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/group-evaluatedynamicmembership-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/group-evaluatedynamicmembership-1-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/group-evaluatedynamicmembership-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面介绍响应示例。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}

```

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a>示例 2：根据成员身份规则评估用户或设备是否为组的成员

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_2"
}-->

```http
POST https://graph.microsoft.com/beta/groups/evaluateDynamicMembership
Content-type: application/json

{
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-2-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-2-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-2-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-2-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-evaluatedynamicmembership-2-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/group-evaluatedynamicmembership-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: evaluateDynamicMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
