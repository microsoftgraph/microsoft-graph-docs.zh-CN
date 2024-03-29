---
title: 列出本地化
description: 从本地化导航属性获取 organizationalBrandingLocalization 资源。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ddc7014b2fb943713e49f0c71b71df6ec2448955
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444445"
---
# <a name="list-localizations"></a>列出本地化
命名空间：microsoft.graph

检索所有本地化品牌对象，包括默认品牌。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | User.Read、Organization.Read.All、User.ReadBasic.All、User.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}/branding/localizations
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法仅 `$select` 支持 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [组织BrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_organizationalbrandinglocalization"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding/localizations/
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-organizationalbrandinglocalization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-organizationalbrandinglocalization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-organizationalbrandinglocalization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-organizationalbrandinglocalization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-organizationalbrandinglocalization-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-organizationalbrandinglocalization-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.organizationalBrandingLocalization)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization('84841066-274d-4ec0-a5c1-276be684bdd3')/branding/localizations",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/$/Microsoft.DirectoryServices.Organization('84841066-274d-4ec0-a5c1-276be684bdd3')//localizations/0",
            "id": "0",
            "backgroundColor": "",
            "backgroundImageRelativeUrl": "c1c6b6c8-ctwpxrbizfcsectmtir3yvna3hrhaib9j7ueqv0ldne/logintenantbranding/0/illustration?ts=637635061764954395",
            "bannerLogoRelativeUrl": "c1c6b6c8-ctwpxrbizfcsectmtir3yvna3hrhaib9j7ueqv0ldne/logintenantbranding/0/bannerlogo?ts=637635061773126717",
            "cdnList": [
                "secure.aadcdn.microsoftonline-p.com",
                "aadcdn.msftauthimages.net",
                "aadcdn.msauthimages.net"
            ],
            "signInPageText": "Contoso",
            "squareLogoRelativeUrl": "c1c6b6c8-ctwpxrbizfcsectmtir3yvna3hrhaib9j7ueqv0ldne/logintenantbranding/0/tilelogo?ts=637635061781098977",
            "usernameHintText": ""
        },
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/$/Microsoft.DirectoryServices.Organization('84841066-274d-4ec0-a5c1-276be684bdd3')//localizations/fr",
            "id": "fr",
            "backgroundColor": "#FFFF33",
            "backgroundImageRelativeUrl": null,
            "bannerLogoRelativeUrl": null,
            "cdnList": [],
            "signInPageText": "Welcome",
            "squareLogoRelativeUrl": null,
            "usernameHintText": "hint"
        }
    ]
}
```

