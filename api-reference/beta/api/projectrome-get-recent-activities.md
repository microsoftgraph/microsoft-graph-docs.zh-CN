---
title: 获取最近的用户活动
description: " #c1. 该服务将查询最近的 historyItems, 然后拉出这些相关的活动。 活动将根据**historyItem**上的最新**lastModified**进行排序。 这意味着不会在响应中包含不含**historyItems**的活动。 useractivity.readwrite.createdbyapp 权限还将对响应应用额外的筛选, 以便仅返回应用程序所创建的活动。 如果用户特别是活动的, 并且其他应用程序已创建了更新的活动, 则此服务器端筛选可能会导致空页面。 若要获取应用程序的活动, 请使用**nextLink**属性进行分页。"
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 464d57e5257b1e9c85796e72e4b8cbda732d4946
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337189"
---
# <a name="get-recent-user-activities"></a>获取最近的用户活动

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取给定用户的最近活动。 此 OData 函数包含一些默认行为, 以使其像 "最近使用过的" API 一样运行。 该服务将查询最近的[historyItems](../resources/projectrome-historyitem.md), 然后拉出这些相关的活动。 活动将根据**historyItem**上的最新**lastModified**进行排序。 这意味着不会在响应中包含不含**historyItems**的活动。 useractivity.readwrite.createdbyapp 权限还将对响应应用额外的筛选, 以便仅返回应用程序所创建的活动。 如果用户特别是活动的, 并且其他应用程序已创建了更新的活动, 则此服务器端筛选可能会导致空页面。 若要获取应用程序的活动, 请使用**nextLink**属性进行分页。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | UserActivity.ReadWrite.CreatedByApp    |
|委派（个人 Microsoft 帐户） | UserActivity.ReadWrite.CreatedByApp    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。 支持以下查询参数:

- **historyItems**导航属性的 $expand。
- $top, 以限制跨页的最大项目数。
- 在**活动**或**historyItems**的**lastModifiedDateTime**属性上 $filter (如果已展开)。

以下是使用 URL 编码支持的查询的一些示例。

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a>请求标头

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|Authorization | string | Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿指定请求正文。

## <a name="response"></a>响应

如果成功, 此方法将返回`200 OK`应用程序的用户最近活动的响应代码。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a>响应

下面是一个响应示例。

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.activity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": "false",
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "https://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "https://www.contoso.com/article?id=12345",
        "contentUrl": "https://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "https://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
