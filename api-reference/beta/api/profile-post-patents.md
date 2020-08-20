---
title: 创建首要项目
description: 创建新的父对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8345de1ca41dfd5e338b77c667ef06ae4b3bf31c
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820285"
---
# <a name="create-itempatent"></a>创建 itemPatent

命名空间：microsoft.graph

在用户的 [配置文件中创建新的 itemPatent](../resources/itempatent.md) [对象](../resources/profile.md)。

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
POST /me/profile/patents
POST /users/{id | userPrincipalName}/profile/patents
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [itemPatent 对象的](../resources/itempatent.md) JSON 表示形式。

下表显示在用户的配置文件中创建新 [itemPatent](../resources/itempatent.md) 对象时可能设置 [的属性](../resources/profile.md)。

|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|description|String|专利或分级说明。 |
|displayName|String|表示属性或下事的标题。 |
|推据|[inferenceData](../resources/inferencedata.md)|如果实体受到创建或修改的应用程序的推理，则包含推理详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|isPending        |Boolean     |表示 Patent 正在挂起。        |
|issuedDate       |日期        |获取该属性的日期。   |
|issuingAuthority |String      |授予 Patent 权限的颁发机构。     |
|数字           |String      |Patent 数。                      |
|source|[personDataSource](../resources/persondatasource.md)|同步到其他服务时从哪个位置发送值。 继承自 [itemFacet](../resources/itemfacet.md)。|
|webUrl           |String      |引用 patent 或 Filing 的 URL。 |

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 [响应代码和 itemPatent](../resources/itempatent.md) 对象。

## <a name="examples"></a>示例

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itempatent_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/patents
Content-Type: application/json
Content-length: 497

{
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempatent-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempatent-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempatent-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "me",
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
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "issuedDate": "Date",
  "issuingAuthority": null,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
