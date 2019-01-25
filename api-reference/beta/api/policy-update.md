---
title: 更新策略
description: 更新以前存在策略中的属性。
localization_priority: Normal
ms.openlocfilehash: d99aa42c4a67f6b874cbc1e266da76287388c05e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515410"
---
# <a name="update-policy"></a>更新策略

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新以前存在[策略](../resources/policy.md)中的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type | application/json  | 实体正文中的数据性质。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，将一个 JSON 对象，提供需要更新的参数。 下表显示可能的参数。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|definition|String|Stringified 的[策略](../resources/policy.md)对象的版本。|
|displayName|String|自定义策略名称。|
|isOrganizationDefault|Boolean|指定默认情况下是否应用此策略。|
|type|String|指定策略的类型。 当前值必须为"TokenLifetimePolicy"|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。 如果不成功，`4xx`与特定的详细信息，则返回错误。

## <a name="example"></a>示例
以下示例更新的令牌生存期策略定义，并将其设置为默认组织。

##### <a name="request"></a>请求
下面是一个请求示例。

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
