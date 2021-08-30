---
title: 获取 samlOrWsFedExternalDomainFederation
description: 读取 samlOrWsFedExternalDomainFederation 对象的属性和关系。
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2622ab603d45fe85f2101441ea22380a80f41cc8
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697048"
---
# <a name="get-samlorwsfedexternaldomainfederation"></a>获取 samlOrWsFedExternalDomainFederation
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取特定[externalDomainName](../resources/externaldomainname.md)[的 samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)对象的属性和关系。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|Domain.Read.All、Domain.ReadWrite.All|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序|Domain.Read.All、Domain.ReadWrite.All|

工作或学校帐户需要属于 Azure AD 角色Azure Active Directory ([之) 之一](/azure/active-directory/roles/permissions-reference)：

* 全局管理员
* 外部标识提供程序管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation?$filter=domains/any(x: x/id eq 'domainName-value')
```

## <a name="query-parameters"></a>查询参数

此方法需要 `$filter` OData 查询参数。 若要检索基于[externalDomainName](../resources/externaldomainname.md)的特定[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)筛选器，请添加 `?$filter=domains/any(x: x/id eq 'domainName-value')` 。 

若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_samlorwsfedexternaldomainfederation"
}
-->

``` http
GET https://graph.microsoft.com/beta/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation?$filter=domains/any(x: x/id eq 'contoso.com')
```

### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "id": "96db02e2-80c1-5555-bc3a-de92ffb8c5be",
        "displayName": "Contoso",
        "issuerUri": "http://contoso.com/adfs/services/trust",
        "metadataExchangeUri": null,
        "signingCertificate": "MIIC6DCCAdCgAwIBAgIQQ6vYJIVKQ",
        "passiveSignInUri": "https://contoso.com/adfs/ls/",
        "preferredAuthenticationProtocol": "saml",
        "domains": [
            {
                "id": "contoso.com"
            }
        ]
    }
  ]
}

```
