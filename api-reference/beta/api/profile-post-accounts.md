---
title: 创建帐户
description: 创建新的帐户对象。
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e08059b08eba1b919a1320627e9ff8bc114d410f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132894"
---
# <a name="create-account"></a>创建帐户
命名空间：microsoft.graph

在用户配置文件中创建新的 [userAccountInformation](../resources/useraccountinformation.md) [对象](../resources/profile.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | User.ReadWrite、User.ReadWrite.All          |
| 委派（个人 Microsoft 帐户） | User.ReadWrite、User.ReadWrite.All          |
| 应用程序                            | User.ReadWrite.All                          |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/account
POST /users/{id | userPrincipalName}/profile/account
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userAccountInformation](../resources/useraccountinformation.md) 对象的 JSON 表示形式。

下表显示创建新的 [userAccountInformation](../resources/useraccountinformation.md) 对象时所需的属性。

|属性|类型|Description|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|countryCode|String|包含与用户帐户关联的两个字符的国家/地区代码。  |
|inference|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|preferredLanguageTag|[localeInfo](../resources/localeinfo.md)|包含用户关联为帐户首选的语言。   |
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值源自何处。 继承自 [itemFacet](../resources/itemfacet.md)。|

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应 [代码和 userAccountInformation](../resources/useraccountinformation.md) 对象。

## <a name="examples"></a>示例


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_useraccountinformation_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/account
Content-Type: application/json

{
  "allowedAudiences": "organization",
  "countryCode": "NO",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-useraccountinformation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-useraccountinformation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-useraccountinformation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-useraccountinformation-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-useraccountinformation-from-profile-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-useraccountinformation-from-profile-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
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
  "ageGroup": "adult",
  "countryCode": "NO",
  "preferredLanguageTag": null,
  "userPrincipalName": "innocenty.popov@adventureworks.com"
}
```


