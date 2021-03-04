---
title: 创建 authenticationListener
description: 为 onSignUpStart 事件创建新的 authenticationListener 对象。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c24ceff80c873181799ea38fbe23c6054f876bc7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438531"
---
# <a name="create-authenticationlistener"></a>创建 authenticationListener

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为 onSignUpStart 事件创建新的 authenticationListener 对象。

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
POST /identity/events/onSignupStart
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [authenticationListener](../resources/authenticationlistener.md) 对象的 JSON 表示形式。

下表显示创建 [invokeUserFlowListener authenticationListener](../resources/invokeuserflowlistener.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|priority|Int32|侦听器的优先级。 确定事件具有多个侦听器时的评估顺序。 优先级从低到高计算。|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|基于用于确定是否评估侦听器的身份验证源的筛选器。 这目前仅限于基于用户进行身份验证的应用程序的评估。|
|userFlow|[b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)|计算此操作时将调用的 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `201 Created` [authenticationListener](../resources/authenticationlistener.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "create_authenticationlistener_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/events/onSignupStart
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.invokeUserFlowListener",
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

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationListener"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/events/onSignupStart/Microsoft.Graph.InvokeUserFlowListener/$entity",
    "@odata.type": "#microsoft.graph.invokeUserFlowListener",
    "id": "2be3336b-e3b4-44f3-9128-b6fd9ad39bb8",
    "priority": 101,
    "sourceFilter": {
        "includeApplications": [
            "1fc41a76-3050-4529-8095-9af8897cf63d"
        ]
    }
}
```
