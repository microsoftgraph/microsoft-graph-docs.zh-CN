---
title: assignLicense
description: 添加或删除用户的许可证, 以启用或禁用其对 Microsoft 云产品的使用。 例如, 组织可以拥有具有100许可证的 Office 365 企业版 E3 订阅, 此请求将其中一个许可证分配给特定用户。 还可以启用和禁用与订阅相关的特定计划。 若要了解有关订阅和许可证的详细信息, 请参阅此 Technet 文章。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3f0d5742417bcd08c5faf83a51b28b2e0d548986
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270488"
---
# <a name="assignlicense"></a>assignLicense

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添加或删除用户的许可证, 以启用或禁用其对 Microsoft 云产品的使用。 例如, 组织可以拥有具有100许可证的 Office 365 企业版 E3 订阅, 此请求将其中一个许可证分配给特定用户。 还可以启用和禁用与订阅相关的特定计划。 若要了解有关订阅和许可证的详细信息, 请参阅此[Technet 文章](https://technet.microsoft.com/en-us/library/mt765146.aspx)。

若要获取目录中可用的订阅, 请执行[Get subscribedsku 请求](subscribedsku-list.md)。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | User.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|addLicenses|[assignedLicense](../resources/assignedlicense.md) 集合|用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。 您可以通过在[assignedLicense](../resources/assignedlicense.md)对象上设置**disabledPlans**属性来禁用与许可证关联的 servicePlans。|
|removeLicenses|Guid 集合|标识要删除的许可证的 skuIds 的集合。|

## <a name="response"></a>响应

如果成功, 此方法在`200 OK`响应正文中返回响应代码和更新的[user](../resources/user.md)对象。

## <a name="example"></a>示例
向用户添加许可证。
##### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```

## <a name="example"></a>示例
删除用户的许可证。

##### <a name="request"></a>请求
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/user_assignlicense-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_assignlicense-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_assignlicense-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="response"></a>响应
在这两个示例中, 响应是更新的用户对象。 注意：为简洁起见，可能会截断此处显示的响应对象。 将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
