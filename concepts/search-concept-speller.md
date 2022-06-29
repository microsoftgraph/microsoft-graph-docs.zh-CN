---
title: 使用 Microsoft 搜索 API 请求拼写更正
description: 使用 Microsoft Graph 中的 Microsoft 搜索 API 请求拼写更正，以处理用户查询中的拼写错误与匹配内容中的正确单词之间的不匹配。
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 16375f1c0e38cc5e0acf3f2f89e668d32a042e51
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438260"
---
# <a name="use-the-microsoft-search-api-to-request-spelling-corrections"></a>使用 Microsoft 搜索 API 请求拼写更正

可以使用 Microsoft Graph 中的 Microsoft 搜索 API 请求拼写更正，以处理用户查询中的拼写错误与匹配内容中的正确单词之间的不匹配。 若要请求拼写更正，请在 [searchRequest](/graph/api/resources/searchrequest) 的 **queryAlterationOptions** 属性中指定以下属性：

- **enableSuggestion** 为用户查询启用/禁用拼写建议。 可以传递 `true` 以获取用户查询中拼写错误的建议拼写更正信息。

- **enableModification** ，为用户查询启用/禁用拼写修改。 如果原始查询没有带拼写错误的结果，则可以传递 `true` 以获取已更正查询的搜索 *结果* ，并获取相应的更正信息。

如果两者都已启用，则拼写修改的优先级高于拼写建议。

所有用户查询字符串都应相同，以便为多个实体的搜索启用拼写更正。

## <a name="example-1-request-spelling-suggestions"></a>示例 1：请求拼写建议

以下示例查询包含字符串`accountt`**的 listItem** 资源，并为查询请求拼写建议。

响应包含拼写建议的 [alterationResponse](/graph/api/resources/alterationResponse) 对象。

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

以下示例查询包含字符串`accountt`的 **listItem** 资源，并为查询请求拼写修改。

在此示例中，具有拼写错误 `accountt`的原始查询没有结果。 响应包含与拼写修改的更正字符串 `account` 和 [alterationResponse](/graph/api/resources/alterationResponse) 对象相关的结果。

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

只有以下资源才支持拼写更正： **消息**、 **事件**、 **站点**、 **驱动器**、 **driveItem**、 **list**、 **listItem** 和 **externalItem**。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview)
