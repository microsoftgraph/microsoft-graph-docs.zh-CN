---
title: 列出 onSignUpStart 侦听器
description: 获取 onSignupStart 事件支持的 authenticationListener 资源的集合。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e8a9df7abd1229b38c0939372f6595a2bd4f073b
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764638"
---
# <a name="list-onsignupstart-listeners"></a>列出 onSignUpStart 侦听器

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 onSignupStart 事件支持的 authenticationListener 资源的集合。 onSignUpStart 事件支持 [invokeUserFlowListener](../resources/invokeuserflowlistener.md) 类型。

当[将 invokeUserFlowListener](../resources/invokeuserflowlistener.md)分配给 onSignUpStart 事件时，应用程序会与用户流关联，因此在它上启用自助服务[](/azure/active-directory/external-identities/self-service-sign-up-overview)注册过程。 创建用于调用用户流的身份验证事件后，转到该应用程序的用户将能够启动设置来宾帐户的注册流。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$expand` OData 查询参数扩展 invokeUserFlowListener 的详细信息。 有关示例，请参阅下文。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [authenticationListener](../resources/authenticationlistener.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-list-authenticationlisteners-for-the-onsignupstart-event"></a>示例 1：列出 onSignUpStart 事件的 authenticationListeners

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "list_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart
```

#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.authenticationListener)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart",
  "value": [
    {
      "@odata.type": "#microsoft.graph.invokeUserFlowListener",
      "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
      "priority": 101,
      "sourceFilter": {
        "includeApplications": [
            "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
        ]
      }
    },
    {
      "@odata.type": "#Microsoft.Graph.InvokeUserFlowListener",
      "id": "0a09997f-fa0c-4f3c-9d02-76762ac069c8",
      "priority": 100,
      "sourceFilter": {
          "includeApplications": [
              "b0e1638f-4c39-4cd1-82b3-91d1caef65f8"
        ]
      }
    }
  ]
}
```

### <a name="example-2-expand-invokeuserflowlisteners-in-authenticationlisteners-for-the-onsignupstart-event"></a>示例 2：展开 onSignUpStart 事件的 authenticationListeners 中的 invokeUserFlowListeners

以下示例列出为 onSignupStart 事件定义的侦听器，并针对每个侦听器扩展调用的用户流。

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "list_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart?$expand=microsoft.graph.invokeUserFlowListener/userFlow
```

#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.invokeUserFlowListener)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart(microsoft.graph.invokeUserFlowListener/userFlow())/$entity",
  "value": [
    {
      "@odata.type": "#microsoft.graph.invokeUserFlowListener",
      "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
      "priority": 101,
      "sourceFilter": {
        "includeApplications": [
            "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
        ]
      },
      "userFlow": {
            "id": "B2X_1_Partner",
            "userFlowType": "signUpOrSignIn",
            "userFlowTypeVersion": 1
      }
    },
    {
      "@odata.type": "#microsoft.graph.InvokeUserFlowListener",
      "id": "0a09997f-fa0c-4f3c-9d02-76762ac069c8",
      "priority": 100,
      "sourceFilter": {
        "includeApplications": [
            "b0e1638f-4c39-4cd1-82b3-91d1caef65f8"
        ]
      },
      "userFlow": {
            "id": "B2X_1_Partner",
            "userFlowType": "signUpOrSignIn",
            "userFlowTypeVersion": 1
      }
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List onSignUpStart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_authenticationlistener_invokeuserflowlistener/container/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_authenticationlistener_invokeuserflowlistener/container/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
