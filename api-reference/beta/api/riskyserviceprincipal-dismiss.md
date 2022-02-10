---
title: riskyServicePrincipal：消除
description: 消除一个或多个 riskyServicePrincipal 对象的风险。
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6bdb0100d017fbb53d796520dfab5b4766da7afc
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519940"
---
# <a name="riskyserviceprincipal-dismiss"></a>riskyServicePrincipal：消除
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

消除一个或多个 [riskyServicePrincipal 对象](../resources/riskyserviceprincipal.md) 的风险。 此操作将目标服务主体帐户的风险级别设定为 `none`。 一个请求中可以消除最多 60 个服务主体帐户。

>**注意：** 使用 riskyServicePrincipal API 需要一个Azure AD Premium P2许可证。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|IdentityRiskyServicePrincipal.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|IdentityRiskyServicePrincipal.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyServicePrincipals/dismiss
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
在请求正文中，在 **servicePrincipalIds** 属性中指定风险服务主体的 ID 集合。 

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。 它不会在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "riskyserviceprincipal_dismiss"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityProtection/riskyServicePrincipals/dismiss
Content-Type: application/json

{
  "servicePrincipalIds": [
    "9089a539-a539-9089-39a5-899039a58990"
  ]
}
```


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

