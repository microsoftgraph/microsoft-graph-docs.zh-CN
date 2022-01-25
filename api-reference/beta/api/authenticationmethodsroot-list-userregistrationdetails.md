---
title: 列出 userRegistrationDetails
description: 获取为用户注册的身份验证方法的列表，如 userRegistrationDetails 对象中的定义。
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 3eb086776644d712f3443554df741ca2a85748aa
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201760"
---
# <a name="list-userregistrationdetails"></a>列出 userRegistrationDetails
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取为用户注册的身份验证方法的列表，如 [userRegistrationDetails](../resources/userregistrationdetails.md) 对象中的定义。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|UserAuthenticationMethod.Read.All、AuditLog.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|UserAuthenticationMethod.Read.All、AuditLog.Read.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/userRegistrationDetails
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法仅支持 `$filter` 和 `$orderBy` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userRegistrationDetails](../resources/userregistrationdetails.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_userregistrationdetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/userRegistrationDetails
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userRegistrationDetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userRegistrationDetails",
      "id": "6832a83d-2ef9-c5f5-9a2d-f2761d7ff317",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "isMfaRegistered": "Boolean",
      "isMfaCapable": "Boolean",
      "isSsprRegistered": "Boolean",
      "isSsprEnabled": "Boolean",
      "isSsprCapable": "Boolean",
      "isPasswordlessCapable": "Boolean",
      "methodsRegistered": [
        "String"
      ]
    }
  ]
}
```

