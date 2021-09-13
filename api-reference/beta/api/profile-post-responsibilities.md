---
title: 创建责任
description: 创建新的责任对象。
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4202dbcfd268ac7e77a1d6e02865b0ed4a4b2774
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59141408"
---
# <a name="create-personresponsibility"></a>创建 personResponsibility
命名空间：microsoft.graph

在用户配置文件 [中创建新的 personResponsibility](../resources/personresponsibility.md) [对象](../resources/profile.md)。

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
POST /me/responsibilities
POST /users/{id | userPrincipalName}/responsibilities
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [personResponsibility](../resources/personresponsibility.md) 对象的 JSON 表示形式。

下表显示了在用户配置文件中的新 [personResponsibility](../resources/personresponsibility.md) 对象中可以设置 [的属性](../resources/profile.md)。

|属性|类型|说明|
|:---|:---|:---|
|allowedAudiences|String|能够查看实体中包含的值的访问群体。 继承自 [itemFacet](../resources/itemfacet.md)。 可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。|
|collaborationTags|字符串集合|包含用户与兴趣相关联的体验方案标记。 集合中允许的值为 `askMeAbout` `ableToMentor` ：、、、。 `wantsToLearn` `wantsToImprove`|
|说明|String|责任说明。|
|displayName|String|包含该责任的友好名称。 |
|inference|[inferenceData](../resources/inferencedata.md)|如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。 继承自 [itemFacet](../resources/itemfacet.md)。|
|source|[personDataSource](../resources/persondatasource.md)|如果从另一个服务同步，则值源自何处。 继承自 [itemFacet](../resources/itemfacet.md)。|
|WebUrl|String|包含指向有关责任的网页或资源的链接。|

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [personResponsibility](../resources/personannotation.md) 对象。

## <a name="examples"></a>示例


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personresponsibility_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/responsibilities
Content-Type: application/json
Content-length: 413

{
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "collaborationTags": [
    "askMeAbout"
  ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personresponsibility-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personresponsibility-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
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
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```


