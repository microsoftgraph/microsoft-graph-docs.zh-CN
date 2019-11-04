---
title: 获取 projectParticipation
description: 检索 projectParticipation 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d3c37c0743bd9d1d9eccf0d35584dc537938ca07
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937628"
---
# <a name="get-projectparticipation"></a>获取 projectParticipation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在用户的[配置文件](../resources/profile.md)中检索[projectParticipation](../resources/projectparticipation.md)对象的属性和关系。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| 委派（工作或学校帐户）     | User. Read、User.readbasic.all、user. all、All、user. all。 All |
| 委派（个人 Microsoft 帐户） | User. Read、User.readbasic.all、user. all、All、user. all。 All |
| Application                            | User.readbasic.all、所有用户读写全部。 All                            |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/projects/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持以下 OData 查询参数来帮助自定义响应。 有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。

|名称            |值    |说明                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|$filter         |string   |将响应限制为仅包含指定条件的那些对象。                                                                                             |
|$orderby        |string   |默认情况下，响应中的对象按其在查询中的**createdDateTime**值进行排序。 您可以使用`$orderby`参数更改响应的顺序。|
|$select         |string   |要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。                                        |
|$skip           |int      |跳过前 n 个结果，对于分页非常有用。                                                                                                                                |
|$top            |int      |要返回的结果数。                                                                                                                                           |

## <a name="request-headers"></a>请求标头

| 名称           |说明                  |
|:---------------|:----------------------------|
| Authorization  | Bearer {token}。必需。   |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[projectParticipation](../resources/projectparticipation.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_projectparticipation"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/projects/{id}
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get projectParticipation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
