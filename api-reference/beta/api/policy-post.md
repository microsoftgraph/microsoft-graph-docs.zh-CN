---
title: 创建策略
description: 通过指定显示名称、 策略类型和策略说明创建新的策略对象。
localization_priority: Normal
ms.openlocfilehash: 4850b2899bfd9add703af912f16602960b2657f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831232"
---
# <a name="create-policy"></a>创建策略

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

通过指定显示名称、 策略类型和策略说明创建新的[策略](../resources/policy.md)对象。

>注意： 将被存储之前验证策略的详细信息。 如果它未通过验证，400 错误的请求将返回。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

```http
POST /policies
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type | application/json  | 实体正文中的数据性质。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供了[策略](../resources/policy.md)对象的 JSON 表示形式。

下表显示当您创建策略时所需的属性。

| 参数    | 类型   |Description|
|:---------------|:--------|:----------|
|definition|字符串|[策略](../resources/policy.md)对象的字符串版本。|
|displayName|字符串|自定义策略名称。|
|type|字符串|指定策略的类型。 当前值必须为"TokenLifetimePolicy"|

## <a name="response"></a>响应

如果成功，此方法返回`201 Created`响应正文中的响应代码和[策略](../resources/policy.md)对象。 如果不成功，`4xx`与特定的详细信息，则返回错误。  

## <a name="example"></a>示例
下面的示例创建新的令牌生存期策略。 请注意字符串定义参数具有转义双引号括起来。

##### <a name="request"></a>请求
下面是一个请求示例。

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
  "id":"id-value",
  "alternativeIdentifier":null,
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "displayName":"name-value",
  "isOrganizationDefault":false,
  "keyCredentials",
  "type":"TokenLifetimePolicy"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
