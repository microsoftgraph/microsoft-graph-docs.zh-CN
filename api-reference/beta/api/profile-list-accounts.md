---
title: 列出帐户
description: 检索 userAccountInformation 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 44727e74b249828124413c120eb458cd0fd2b5a6
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292432"
---
# <a name="list-accounts"></a>列出帐户

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从配置文件中检索与用户帐户相关的 [属性](../resources/profile.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| 委派（工作或学校帐户）     | User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All |
| 应用程序                            | User.ReadBasic.All、User.Read.All、User.ReadWrite.All                            |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account
GET /users/{id | userPrincipalName}/profile/account
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持以下 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

|名称            |值    |说明                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|$filter         |string   |将响应限制到仅包含指定条件的对象。                                                                                             |
|$orderby        |string   |默认情况下，响应中的对象按查询中的 createdDateTime 值进行排序。 可以使用 $orderby 参数更改 *响应* 的顺序。|
|$select         |string   |要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。                                        |
|$skip           |int      |跳过前 n 个结果，对分页很有用。                                                                                                                                |
|$top            |int      |要返回的结果数。                                                                                                                                           |


## <a name="request-headers"></a>请求标头

| 名称           |说明                  |
|:---------------|:----------------------------|
| Authorization  | Bearer {token}。必需。   |
| Content-Type   | application/json. Required. |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `200 OK` [userAccountInformation](../resources/useraccountinformation.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "get_account"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/account
```


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```


