---
title: 删除 authenticationListener
description: 从 authenticationEventsPolicy 支持的事件中删除 authenticationListener。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3db702f80e92ce475d0b3699236096d7d7b79392
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872322"
---
# <a name="remove-authenticationlistener"></a>删除 authenticationListener

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除为身份验证管道中的 onSignupStart 事件定义的指定[authenticationListener。](../resources/authenticationlistener.md)

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
DELETE /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "delete_onsignupstart_from_authenticationeventspolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
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
