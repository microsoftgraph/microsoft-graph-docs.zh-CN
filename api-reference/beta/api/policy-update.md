---
title: 更新策略
description: 更新预先存在的策略中的属性。
localization_priority: Normal
ms.openlocfilehash: d99aa42c4a67f6b874cbc1e266da76287388c05e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538736"
---
# <a name="update-policy"></a>更新策略

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新预先存在的[策略](../resources/policy.md)中的属性。

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
在请求正文中, 提供具有需要更新的参数的 JSON 对象。 下表显示了可能的参数。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|定义|String|[policy](../resources/policy.md)对象的字符串化版本。|
|displayName|String|策略的自定义名称。|
|isOrganizationDefault|布尔值|指定默认情况下是否应用此策略。|
|类型|String|指定策略的类型。 当前必须是 "TokenLifetimePolicy"|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="example"></a>示例
下面的示例更新令牌生存期策略的定义, 并将其设置为组织的默认值。

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
