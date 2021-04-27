---
title: 创建 personInterest
description: 创建新的 personInterest。
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: e4f5648901ff1ed904d5e02fa278b6b9be329de8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036924"
---
# <a name="create-personinterest"></a>创建 personInterest

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [personInterest] (。/resources/personinterest.md] in a [user's profile](../resources/profile.md).

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | User.ReadWrite、User.ReadWrite.All          |
| 委派（个人 Microsoft 帐户） | User.ReadWrite、User.ReadWrite.All          |
| 应用程序                            | User.ReadWrite.All                          |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/interests
POST /users/{id | userPrincipalName}/profile/interests
```

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。|
| Content-Type   | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [personInterest](../resources/personinterest.md) 对象的 JSON 表示形式。

下表显示了在用户配置文件中的新 [personInterest](../resources/personinterest.md) 对象中可以设置 [的属性](../resources/profile.md)。

|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|categories|String 集合|包含用户与兴趣类别关联的类别 (例如个人、) 。 |
|collaborationTags|字符串集合|包含用户与兴趣相关联的体验方案标记。 集合中允许的值为 `askMeAbout` `ableToMentor` ：、、、。 `wantsToLearn` `wantsToImprove`|
|说明|String|包含感兴趣的说明。|
|displayName|String|包含兴趣的友好名称。  |
|inference|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值源自何处。 继承自 [itemFacet](../resources/itemfacet.md)。|
|webUrl|String|包含指向有关感兴趣的网页或资源的链接。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [personInterest](../resources/personinterest.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personinterest_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/interests
Content-type: application/json

{
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personinterest-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```


