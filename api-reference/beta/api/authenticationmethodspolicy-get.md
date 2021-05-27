---
title: 获取 authenticationMethodsPolicy
description: 读取 authenticationMethodsPolicy 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b54b95f3db35d744d400fb50a221cdfdad12890b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682874"
---
# <a name="get-authenticationmethodspolicy"></a>获取 authenticationMethodsPolicy
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.AuthenticationMethod|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Policy.ReadWrite.AuthenticationMethod|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法不支持任何可选的查询参数。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethodspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#authenticationMethodsPolicy",
    "id": "authenticationMethodsPolicy",
    "displayName": "Authentication Methods Policy",
    "description": "The tenant-wide policy that controls which authentication methods are allowed in the tenant, authentication method registration requirements, and self-service password reset settings",
    "lastModifiedDateTime": "2021-05-24T18:02:30.5288302Z",
    "policyVersion": "1.4",
    "registrationEnforcement": {
        "authenticationMethodsRegistrationCampaign": {
            "snoozeDurationInDays": 2,
            "state": "enabled",
            "excludeTargets": [],
            "includeTargets": [
                {
                    "id": "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
                    "targetType": "group",
                    "targetedAuthenticationMethod": "microsoftAuthenticator"
                }
            ]
        }
    }
}
```
