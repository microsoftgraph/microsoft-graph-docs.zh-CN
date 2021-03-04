---
title: 更新 authenticationListener
description: 更新为身份验证管道中的事件定义的侦听器。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 65e5fa8252bdb4b25c1992282f655f532f66e1f3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438426"
---
# <a name="update-authenticationlistener"></a>更新 authenticationListener

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新为身份验证管道中的事件定义的[authenticationListener。](../resources/authenticationlistener.md)

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.ApplicationConfiguration|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|Policy.ReadWrite.ApplicationConfiguration|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [authenticationListener](../resources/authenticationlistener.md) 对象的 JSON 表示形式。

下表显示更新 [invokeUserFlowAction](../resources/invokeuserflowlistener.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|priority|Int32|侦听器的优先级。 确定事件具有多个侦听器时的评估顺序。 优先级从低到高计算。|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|基于用于确定是否评估侦听器的身份验证源的筛选器。 这当前仅限于基于用户进行身份验证的应用程序的评估。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "update_onsignupstart"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
Content-Type: application/json

{
  "priority": 101
}
```

### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
