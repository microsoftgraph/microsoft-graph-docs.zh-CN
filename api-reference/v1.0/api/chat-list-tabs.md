---
title: 列出聊天中的选项卡
description: '检索指定聊天中的选项卡列表。 '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1ddf7286d0e806665bbe3eacd1b9cf134fcc1e53
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954884"
---
# <a name="list-tabs-in-chat"></a>列出聊天中的选项卡

命名空间：microsoft.graph

检索指定 [聊天中的](../resources/teamstab.md) 选项卡 [列表](../resources/chat.md)。

> **注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则实际上，将列出固定在会议中的选项卡。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | TeamsTab.ReadWriteForChat、TeamsTab.Read.All、TeamsTab.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | TeamsTab.ReadWriteForChat.All、TeamsTab.Read.All、TeamsTab.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /chats/{chat-id}/tabs
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [tabs](../resources/teamstab.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-list-all-the-tabs-in-the-chat-along-with-associated-teams-app"></a>示例 1：列出聊天中的所有选项卡以及关联的 Teams 应用
#### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tabs_in_chat"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs?$expand=teamsApp
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tabs-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tabs-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tabs-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tabs-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsTab)"
}
-->

```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "displayName": "My Contoso Tab - updated",
      "sortOrderIndex": "20",
      "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_193fe248-24e6-478f-a66c-ede9ce6dd547?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "teamsApp": {
        "id": "06805b9e-77e3-4b93-ac81-525eb87513b8",
        "displayName": "Contoso",
        "distributionMethod": "store"
      }
    },
    {
      "id": "1f7b40e5-ecdf-40cb-b02e-e785cf71c0e9",
      "displayName": "Website2",
      "teamsAppId": null,
      "sortOrderIndex": "10000100",
      "messageId": "1607411851584",
      "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_44125e1d-04b1-421a-9f45-19d913494b3e?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
      "configuration": {
        "entityId": null,
        "contentUrl": "https://www.bing.com",
        "removeUrl": null,
        "websiteUrl": "https://www.bing.com",
        "dateAdded": "2020-12-08T07:17:29.748Z"
      },
      "teamsApp": {
        "id": "com.microsoft.teamspace.tab.web",
        "externalId": null,
        "displayName": "Website",
        "distributionMethod": "store"
      }
    },
    {
      "id": "b92dd123-1624-425c-a808-2f11e03534a5",
      "displayName": "Some random board",
      "sortOrderIndex": "10000100100",
      "messageId": "1607412162267",
      "webUrl": "https://teams.microsoft.com/l/entity/49e6f432-d79c-49e8-94f7-89b94f3672fd/_djb2_msteams_prefix_2919ec48-12d8-4533-b849-56c4d207734b?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
      "configuration": {
        "entityId": "5fcf29c17a3a3142160b8694",
        "contentUrl": "https://trello.com/integrations/teams/tab-content?iframeSource=msteams&contentUrl=https%3A%2F%2Ftrello.com%2Fb%2FkS2FslqK%2Fsome-random-board",
        "removeUrl": "https://trello.com/integrations/teams/tab-delete?iframeSource=msteams",
        "websiteUrl": "https://trello.com/b/kS2FslqK/some-random-board",
        "dateAdded": "2020-12-08T07:22:40.001Z"
      },
      "teamsApp": {
        "id": "49e6f432-d79c-49e8-94f7-89b94f3672fd",
        "externalId": null,
        "displayName": "Trello",
        "distributionMethod": "store"
      }
    }
  ]
}
```

### <a name="example-2-list-all-the-tabs-belonging-to-a-specific-app-in-a-chat"></a>示例 2：列出聊天中属于特定应用的所有选项卡
#### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tabs_in_chat_app_filter"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs?$expand=teamsApp&$filter=teamsApp/id eq 'com.microsoft.teamspace.tab.web'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tabs-in-chat-app-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tabs-in-chat-app-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tabs-in-chat-app-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tabs-in-chat-app-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsTab)"
}
-->

```http
HTTP/1.1 200 Success
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/tabs(teamsApp())",
    "@odata.count": 1,
    "value": [
        {
            "id": "1f7b40e5-ecdf-40cb-b02e-e785cf71c0e9",
            "displayName": "Website2",
            "teamsAppId": null,
            "sortOrderIndex": "10000100",
            "messageId": "1607411851584",
            "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_44125e1d-04b1-421a-9f45-19d913494b3e?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
            "configuration": {
                "entityId": null,
                "contentUrl": "https://www.bing.com",
                "removeUrl": null,
                "websiteUrl": "https://www.bing.com",
                "dateAdded": "2020-12-08T07:17:29.748Z"
            },
            "teamsApp": {
                "id": "com.microsoft.teamspace.tab.web",
                "externalId": null,
                "displayName": "Website",
                "distributionMethod": "store"
            }
        }
    ]
}
```

## <a name="see-also"></a>另请参阅

- [列出频道中的选项卡](channel-list-tabs.md)
- 
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List all tabs in chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


