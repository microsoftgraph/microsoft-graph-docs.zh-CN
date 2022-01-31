---
title: 使用 Microsoft Microsoft 搜索中的 Graph API 请求拼写更正
description: 您可以使用 Microsoft 搜索 API 获取搜索查询的拼写建议或拼写修改。
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: c672af903811af716ae7c597bdc748974d24a1e2
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282182"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-request-spelling-correction-preview"></a>使用 Microsoft Microsoft 搜索 中的 Graph API 请求拼写更正 (预览) 

您可以使用 Microsoft 搜索 API 请求拼写更正，以处理用户查询中的拼写错误与匹配内容中的正确单词之间的不匹配。 若要请求拼写更正，在 [searchRequest](/graph/api/resources/searchrequest?view=graph-rest-beta&preserve-view=true) 的 **queryAlterationOptions** 属性中指定以下属性：

- **enableSuggestion** 为用户查询启用/禁用拼写建议。 您可以通过传递 `true` 获取用户查询中拼写错误的建议拼写更正信息。

- **enableModification** 为用户查询启用/禁用拼写修改。 当原始`true`查询没有拼写错误的结果时，可以通过传递 获取更正的查询的搜索结果，并获取相应的更正信息。

如果同时启用了拼写修改，则其优先级高于拼写建议。

所有用户查询字符串应相同，以便对多个实体的搜索启用拼写更正。

## <a name="example-1-request-spelling-suggestions"></a>示例 1：请求拼写建议

下面的示例查询包含字符串"accountt"的 **listItem** 资源，并请求查询的拼写建议。

该响应包含 [拼写建议的更改Response](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) 对象。

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "listItem"
            ],
            "query": {
                "queryString": "accountt"
            },
            "from": 0,
            "size": 25,
            "queryAlterationOptions": {
                "enableSuggestion": true,
                "enableModification": false
            }
        }
    ]
}
```

### <a name="response"></a>响应

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [
                "accountt"
            ],
            "hitsContainers": [
                {
                    "total": 0,
                    "moreResultsAvailable": false
                }
            ],
            "queryAlterationResponse": {
                "@odata.type": "#microsoft.substrateSearch.alterationResponse",
                "originalQueryString": "accountt",
                "queryAlteration": {
                    "@odata.type": "#microsoft.substrateSearch.searchAlteration",
                    "alteredQueryString": "account",
                    "alteredHighlightedQueryString": "account",
                    "alteredQueryTokens": [
                        {
                            "offset": 0,
                            "length": 8,
                            "suggestion": "account"
                        }
                    ]
                },
                "queryAlterationType": "Suggestion"
            }
        }
    ]
}
```

## <a name="example-2-request-spelling-modifications"></a>示例 2：请求拼写修改

下面的示例查询包含字符串"accountt"的 **listItem** 资源，并请求对查询进行拼写修改。

本示例中，没有包含拼写错误"accountt"的原始查询的结果。 该响应包含与更正的字符串"account"和用于拼写修改 [的 modificationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) 对象相关的结果。

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "listItem"
            ],
            "query": {
                "queryString": "accountt"
            },
            "from": 0,
            "size": 25,
            "queryAlterationOptions": {
                "enableSuggestion": true,
                "enableModification": true
            }
        }
    ]
}
```

### <a name="response"></a>响应

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [
                "account"
            ],
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
                            "rank": 1,
                            "summary": "",
                            "resource": {
                                "@odata.type": "#microsoft.graph.listItem",
                                "createdDateTime": "2019-06-10T06:37:43Z",
                                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                                "name": "web_part_test_long Notebook",
                                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/Lists/Issue tracker list/DispForm.aspx?ID=1",
                                "sharepointIds": {
                                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                                    "listItemId": "13"
                                },
                                "createdBy": {
                                    "user": {
                                        "displayName": "System Account"
                                    }
                                },
                                "lastModifiedBy": {
                                    "user": {
                                        "displayName": "System Account"
                                    }
                                },
                                "parentReference": {
                                    "sharepointIds": {
                                        "listId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b"
                                    },
                                    "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                                }
                            }
                        }
                    ]
                }
            ],
            "queryAlterationResponse": {
                "@odata.type": "#microsoft.substrateSearch.alterationResponse",
                "originalQueryString": "accountt",
                "queryAlteration": {
                    "@odata.type": "#microsoft.substrateSearch.searchAlteration",
                    "alteredQueryString": "account",
                    "alteredHighlightedQueryString": "account",
                    "alteredQueryTokens": [
                        {
                            "offset": 0,
                            "length": 8,
                            "suggestion": "account"
                        }
                    ]
                },
                "queryAlterationType": "Modification"
            }
        }
    ]
}
```

## <a name="known-limitations"></a>已知限制

拼写更正仅支持以下资源： **message**、 **event**、 **site**、 **drive**、 **driveItem**、 **list**、 **listItem** 和 **externalItem**。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
