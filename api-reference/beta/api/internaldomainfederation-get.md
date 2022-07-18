---
title: 获取 internalDomainFederation
description: 读取 internalDomainFederation 对象的属性和关系。
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7ff2c212a3d4a16af022f0d757712a01eb182764
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556275"
---
# <a name="get-internaldomainfederation"></a>获取 internalDomainFederation
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [internalDomainFederation](../resources/internaldomainfederation.md) 对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Domain.Read.All、Domain.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|Domain.Read.All、Domain.ReadWrite.All|

必须为调用用户或应用分配全局管理员 [Azure AD 角色](/azure/active-directory/roles/permissions-reference)。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /domains/{domainsId}/federationConfiguration/{internalDomainFederationId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法不支持 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [internalDomainFederation](../resources/internaldomainfederation.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_internaldomainfederation"
}
-->
``` http
GET https://graph.microsoft.com/beta/domains/contoso.com/federationConfiguration/6601d14b-d113-8f64-fda2-9b5ddda18ecc
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-internaldomainfederation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-internaldomainfederation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-internaldomainfederation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-internaldomainfederation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-internaldomainfederation-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-internaldomainfederation-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.internalDomainFederation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.internalDomainFederation",
    "id": "6601d14b-d113-8f64-fda2-9b5ddda18ecc",
    "displayName": "Contoso",
    "issuerUri": "http://contoso.com/adfs/services/trust",
    "metadataExchangeUri": "https://sts.contoso.com/adfs/services/trust/mex",
    "signingCertificate": "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
    "passiveSignInUri": "https://sts.contoso.com/adfs/ls",
    "preferredAuthenticationProtocol": "wsFed",
    "activeSignInUri": "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed",
    "signOutUri": "https://sts.contoso.com/adfs/ls",
    "promptLoginBehavior": "nativeSupport",
    "isSignedAuthenticationRequestRequired": true,
    "nextSigningCertificate": "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
    "signingCertificateUpdateStatus": {
        "certificateUpdateResult": "Success",
        "lastRunDateTime": "2021-08-25T07:44:46.2616778Z"
    },
    "federatedIdpMfaBehavior": "rejectMfaByFederatedIdp"
  }
}
```

