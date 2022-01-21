---
title: 创建认证
description: 创建新的认证对象。
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 41efade5e1d79c2277b5e27f55fae0697e9e600a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132864"
---
# <a name="create-personcertification"></a>创建 personCertification
命名空间：microsoft.graph

在用户配置文件中创建新的 [personCertification](../resources/personcertification.md) [对象](../resources/profile.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| 委派（工作或学校帐户）     | User.ReadWrite、User.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | User.ReadWrite、User.ReadWrite.All |
| 应用程序                            | User.ReadWrite.All                            |
## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/certifications
POST /users/{id | userPrincipalName}/profile/certifications
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [personCertification](../resources/personcertification.md) 对象的 JSON 表示形式。

下表显示了在用户配置文件中创建新的 [personCertification](../resources/personcertification.md) 对象时可以设置 [的属性](../resources/profile.md)。

|属性|类型|Description|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|certificationId  |String      |证书的可引用标识符。 |
|说明      |String      |认证说明。                   |
|displayName      |String      |认证的标题。                         |
|endDate          |日期        |认证到期的日期。            |
|inference|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|issuedDate       |Date        |颁发证书的日期。         |
|issuingAuthority |String      |授予证书的颁发机构。          |
|issuingCompany   |String      |授予证书的颁发机构。          |
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值源自何处。 继承自 [itemFacet](../resources/itemfacet.md)。|
|startDate        |日期        |认证生效的日期。       |
|thumbnailUrl     |String      |引用认证缩略图的 URL。   |
|WebUrl           |String      |引用证书的 URL。                  |

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [personCertification](../resources/personcertification.md) 对象。

## <a name="examples"></a>示例

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personCertification_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/certifications
Content-Type: application/json

{
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personcertification-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personcertification-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personcertification-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personcertification-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-personcertification-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-personcertification-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personCertification"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": null,
  "issuingCompany": null,
  "startDate": "Date",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```


