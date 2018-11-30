---
title: 更新策略
description: 更新以前存在策略中的属性。
ms.openlocfilehash: 426476b5545e511fe2da111acb1f47f38f32c96f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048612"
---
# <a name="update-policy"></a>更新策略

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
|definition|字符串|Stringified 的[策略](../resources/policy.md)对象的版本。|
|displayName|字符串|自定义策略名称。|
|isOrganizationDefault|布尔|指定默认情况下是否应用此策略。|
|type|字符串|指定策略的类型。 当前值必须为"TokenLifetimePolicy"|

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
