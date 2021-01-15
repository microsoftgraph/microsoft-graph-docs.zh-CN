---
title: Put authenticationListener
description: 替换 authenticationListener 对象。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f5b5e1ea73a9f3df1899f92f3675152e04822a3
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872308"
---
# <a name="put-authenticationlistener"></a>Put authenticationListener

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

替换为身份验证管道中的 onSignupStart 事件定义的[authenticationListener。](../resources/authenticationlistener.md)

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.ApplicationConfiguration|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Policy.ReadWrite.ApplicationConfiguration|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [authenticationListener](../resources/authenticationlistener.md) 对象的 JSON 表示形式。

下表显示创建 [invokeUserFlowListener 时所需的属性](../resources/invokeuserflowlistener.md)。

|属性|类型|Description|
|:---|:---|:---|
|priority|Int32|侦听器的优先级。 确定事件具有多个侦听器时的评估顺序。 优先级从低到高进行评估。|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|基于用于确定是否评估侦听器的身份验证源进行筛选。 当前仅限于基于用户进行身份验证的应用程序的评估。|
|userFlow|[b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)|对此操作中调用的用户流对象的引用。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "put_authenticationlistener_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
Content-Type: application/json

{
    "@odata.type": "#Microsoft.Graph.InvokeUserFlowListener",
    "priority": 101,
    "sourceFilter": {
        "includeApplications": [
            "1fc41a76-3050-4529-8095-9af8897cf63d"
        ]
    },
    "userFlow": {
        "id": "B2X_1_Partner"
    }
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
