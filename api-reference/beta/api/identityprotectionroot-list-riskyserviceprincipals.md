---
title: 列出 riskyServicePrincipals
description: 检索 riskyServicePrincipal 对象的属性和关系。
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 37b15a55f76115c7e8dc7584f328b42e4a347f33
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519974"
---
# <a name="list-riskyserviceprincipals"></a>列出 riskyServicePrincipals
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [riskyServicePrincipal 对象的属性和](../resources/riskyserviceprincipal.md) 关系。

>**注意：** 使用 riskyServicePrincipals API 需要一个Azure AD Premium P2许可证。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|IdentityRiskyServicePrincipal.Read.All、IdentityRiskyServicePrincipal.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|IdentityRiskyServicePrincipal.Read.All、IdentityRiskyServicePrincipal.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyServicePrincipals
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 、 `$count`、 `$filter`和 `$select``$top` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [riskyServicePrincipal](../resources/riskyserviceprincipal.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_riskyserviceprincipal"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/riskyServicePrincipals
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.riskyServicePrincipal)"
}
-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyServicePrincipal",
  "value": [
    {
      "id": "9089a539-a539-9089-39a5-899039a58990",
      "accountEnabled": true,
      "isProcessing": false,
      "riskLastUpdatedDateTime": "2021-08-14T13:06:51.0451374Z",
      "riskLevel": "high",
      "riskState": "atRisk",
      "riskDetail": "none",
      "displayName": "Contoso App",
      "appId": "b55552fe-a272-4b56-990b-95038d917878",
      "servicePrincipalType": "Application"
    }
  ]
}
```
