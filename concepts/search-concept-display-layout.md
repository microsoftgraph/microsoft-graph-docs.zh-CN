---
title: 使用 Microsoft 搜索 API 管理搜索结果的布局模板
description: 使用 Microsoft Graph 中的 Microsoft 搜索 API 通过使用自适应卡片模板和Microsoft 365 管理中心以不同的方式显示搜索结果。
author: yiwenwang
ms.author: yiwenwang
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: cc74f41695b4ae7da84efffae7de7e6935f4b8cd
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444297"
---
# <a name="use-the-microsoft-search-api-to-manage-layout-templates-for-search-results"></a>使用 Microsoft 搜索 API 管理搜索结果的布局模板

可以使用 Microsoft Graph 中的 Microsoft 搜索 API 管理搜索结果的布局模板。 搜索显示布局或结果类型是一个规则，它会导致不同类型的搜索结果以不同的方式显示在搜索结果页中。 它包含以下几个方面：

- 要比较每个搜索结果的一个或多个特征或条件，例如搜索结果的结果源或内容类型。
- 用于符合条件的搜索结果的显示模板。显示模板控制满足条件的所有结果在搜索结果页面上的显示和行为方式。 

Microsoft Graph 搜索 API 提供基于 [自适应卡片](https://adaptivecards.io/)的可呈现响应。 通过使用 [自适应卡片模板](https://adaptivecards.io/designer)，客户端可以在不同的画布中呈现不同的搜索结果。

客户可以在[Microsoft 365 管理中心](https://admin.microsoft.com/Adminportal/Home#/MicrosoftSearch/resulttypes)中自定义搜索结果类型。

## <a name="request-example"></a>请求示例

以下示例演示如何通过将 **enableResultTemplate** 属性 `true` 设置为请求协定中来获取用于呈现搜索结果的显示布局或结果模板。

响应显示三个搜索命中，其中两个与 **结果TemplateId** 1603900360618_5XCBK2OXG相关，另一个与 **resultTemplateId** 1603900360618_5XCBK2OXP。 这些 ID 与响应协定中包含的 **resultTemplates** 字典中包含的两个显示布局的键之一匹配。 使用结果模板 ID，可以确定用于呈现每个搜索结果的显示布局。

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "externalItem"
            ],
            "contentSources": [
                "Connectors"
            ],
            "query": {
                "queryString": "*"
            },
            "resultTemplateOptions": {
                "enableResultTemplate": true
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [],
            "hitsContainers": [
                {
                    "total": 1201701,
                    "moreResultsAvailable": true,
                    "hits": [
                        {
                            "hitId": "85437765-b430-434f-a945-38eceead5b93",
                            "rank": 1,
                            "summary": "",
                            "resultTemplateId": "1603900360618_5XCBK2OXG",
                            "resource": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17397",
                                "Title": "[SM00186] Number of tests - Liquid",
                                "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                            }
                        },
                        {
                            "hitId": "85437765-5430-434f-a945-38eceead5b94",
                            "rank": 2,
                            "summary": "",
                            "resultTemplateId": "1603900360618_5XCBK2OXP",
                            "resource": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17398",
                                "Title": "[SM00186] Number of tests - Liquid 2",
                                "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                            }
                        },
                        {
                            "hitId": "85437765-b430-434f-a945-38eceead5b95",
                            "rank": 3,
                            "summary": "",
                            "resultTemplateId": "1603900360618_5XCBK2OXG",
                            "resource": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17399",
                                "Title": "[SM00186] Number of tests - Liquid 3",
                                "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                            }
                        }
                    ]
                }
            ],
            "resultTemplates": {
                "1603900360618_5XCBK2OXG": {
                    "displayName": "Liquid-3",
                    "body": {
                        "type": "AdaptiveCard",
                        "version": "1.0",
                        "body": [
                            {
                                "type": "ColumnSet",
                                "columns": [
                                    {
                                        "type": "Column",
                                        "width": "auto",
                                        "items": [
                                            {
                                                "type": "Image",
                                                "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                "horizontalAlignment": "Center",
                                                "size": "Small"
                                            }
                                        ],
                                        "horizontalAlignment": "Center"
                                    },
                                    {
                                        "type": "Column",
                                        "width": 10,
                                        "items": [
                                            {
                                                "type": "TextBlock",
                                                "text": "[{Title}]({URL})",
                                                "weight": "Bolder",
                                                "color": "Accent",
                                                "size": "Medium",
                                                "maxLines": 3
                                            },
                                            {
                                                "type": "TextBlock",
                                                "text": "{ResultSnippet}",
                                                "maxLines": 3,
                                                "wrap": true
                                            }
                                        ],
                                        "spacing": "Medium"
                                    }
                                ]
                            }
                        ],
                        "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                    }
                },
                "1603900360618_5XCBK2OXP": {
                    "displayName": "Liquid-2",
                    "body": {
                        "type": "AdaptiveCard",
                        "version": "1.0",
                        "body": [
                            {
                                "type": "ColumnSet",
                                "columns": [
                                    {
                                        "type": "Column",
                                        "width": "auto",
                                        "items": [
                                            {
                                                "type": "Image",
                                                "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                "horizontalAlignment": "Center",
                                                "size": "Small"
                                            }
                                        ],
                                        "horizontalAlignment": "Center"
                                    },
                                    {
                                        "type": "Column",
                                        "width": 10,
                                        "items": [
                                            {
                                                "type": "TextBlock",
                                                "text": "[{Title}]({URL})",
                                                "weight": "Bolder",
                                                "color": "Accent",
                                                "size": "Medium",
                                                "maxLines": 3
                                            },
                                            {
                                                "type": "TextBlock",
                                                "text": "{ResultSnippet}",
                                                "maxLines": 3,
                                                "wrap": true
                                            }
                                        ],
                                        "spacing": "Medium"
                                    }
                                ]
                            }
                        ],
                        "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                    }
                }
            }
        }
    ]
}

```

## <a name="web-component-example"></a>Web 组件示例

以下示例演示如何使用自适应卡片模板来呈现搜索结果。

> [!IMPORTANT] 
> 
> 本示例使用的自适应卡片模板版本早于 **2020 年 5 月版本**。 有关详细信息，请参阅：
> - [自适应卡片模板化](/adaptive-cards/templating/)
> - [自适应卡片模板 SDK](/adaptive-cards/templating/sdk)


<!-- markdownlint-disable MD024 -->
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8" />
    <title>Adaptive Cards Example</title>

    <script src="https://unpkg.com/markdown-it@8.4.0/dist/markdown-it.js"></script>
    <script src="https://unpkg.com/adaptivecards/dist/adaptivecards.min.js"></script>

    <script src="https://unpkg.com/adaptivecards-templating@0.1.0-alpha1/dist/adaptivecards-templating.min.js"></script>
    <script src="https://code.jquery.com/jquery-3.6.0.js"
        integrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk=" crossorigin="anonymous"></script>

    <style type="text/css">
        #exampleDiv {
            border: solid 1px black;
        }
    </style>

    <script type="text/javascript">

       function renderCard() {
            var mockdata = this.getMockData();
            var renderTemplates = [];

            // Convert object to map
            var templateDictionary = new Map(Object.entries( mockdata.value[0].resultTemplates));

            for (let hit of mockdata.value[0].hitsContainers[0].hits) {
                renderTemplates.push(this.renderACT(hit, templateDictionary));
            }

            for(let template of renderTemplates){
                document.getElementById('exampleDiv').appendChild(template);
            }
        }

        function renderACT(hit, templateDictionary) {
            var templateId = hit.resultTemplateId;
            // Define a template payload
            var templatePayload = templateDictionary.get(templateId).body;
            var template = new ACData.Template(templatePayload);

            // Expand the template with your `$root` data object.
            // This binds it to the data and produces the final Adaptive Card payload

            console.log(hit.resource);

            // Create a data binding context, and set its $root property to the
            // data object to bind the template to
            var context = new ACData.EvaluationContext();
            context.$root = hit.resource;

            console.log(context);
            var card = template.expand(context);
            // OPTIONAL: Render the card (requires that the adaptivecards library be loaded)

            var adaptiveCard = new AdaptiveCards.AdaptiveCard();
            adaptiveCard.parse(card);
            return adaptiveCard.render();
        }

        function getMockData() {
            return {
                "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.searchResponse)",
                "value": [
                    {
                        "searchTerms": [],
                        "hitsContainers": [
                            {
                                "total": 1201701,
                                "moreResultsAvailable": true,
                                "hits": [
                                    {
                                        "hitId": "85437765-b430-434f-a945-38eceead5b93",
                                        "rank": 1,
                                        "summary": "",
                                        "resultTemplateId": "1603900360618_5XCBK2OXG",
                                        "resource": {
                                            "@odata.type": "#microsoft.graph.externalItem",
                                            "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17397",
                                            "Title": "[SM00186] Number of tests - Liquid",
                                            "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                                        }
                                    },
                                    {
                                        "hitId": "85437765-5430-434f-a945-38eceead5b94",
                                        "rank": 2,
                                        "summary": "",
                                        "resultTemplateId": "1603900360618_5XCBK2OXP",
                                        "resource": {
                                            "@odata.type": "#microsoft.graph.externalItem",
                                            "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17398",
                                            "Title": "[SM00186] Number of tests - Liquid 2",
                                            "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                                        }
                                    },
                                    {
                                        "hitId": "85437765-b430-434f-a945-38eceead5b95",
                                        "rank": 3,
                                        "summary": "",
                                        "resultTemplateId": "1603900360618_5XCBK2OXG",
                                        "resource": {
                                            "@odata.type": "#microsoft.graph.externalItem",
                                            "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17399",
                                            "Title": "[SM00186] Number of tests - Liquid 3",
                                            "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                                        }
                                    }
                                ]
                            }
                        ],
                        "resultTemplates": {
                            "1603900360618_5XCBK2OXG": {
                                "displayName": "Liquid-3",
                                "body": {
                                    "type": "AdaptiveCard",
                                    "version": "1.0",
                                    "body": [
                                        {
                                            "type": "ColumnSet",
                                            "columns": [
                                                {
                                                    "type": "Column",
                                                    "width": "auto",
                                                    "items": [
                                                        {
                                                            "type": "Image",
                                                            "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                            "horizontalAlignment": "Center",
                                                            "size": "Small"
                                                        }
                                                    ],
                                                    "horizontalAlignment": "Center"
                                                },
                                                {
                                                    "type": "Column",
                                                    "width": 10,
                                                    "items": [
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "[{Title}]({URL})",
                                                            "weight": "Bolder",
                                                            "color": "Accent",
                                                            "size": "Medium",
                                                            "maxLines": 3
                                                        },
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "{ResultSnippet}",
                                                            "maxLines": 3,
                                                            "wrap": true
                                                        }
                                                    ],
                                                    "spacing": "Medium"
                                                }
                                            ]
                                        }
                                    ],
                                    "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                                }
                            },
                            "1603900360618_5XCBK2OXP": {
                                "displayName": "Liquid-2",
                                "body": {
                                    "type": "AdaptiveCard",
                                    "version": "1.0",
                                    "body": [
                                        {
                                            "type": "ColumnSet",
                                            "columns": [
                                                {
                                                    "type": "Column",
                                                    "width": "auto",
                                                    "items": [
                                                        {
                                                            "type": "Image",
                                                            "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                            "horizontalAlignment": "Center",
                                                            "size": "Small"
                                                        }
                                                    ],
                                                    "horizontalAlignment": "Center"
                                                },
                                                {
                                                    "type": "Column",
                                                    "width": 10,
                                                    "items": [
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "[{Title}]({URL})",
                                                            "weight": "Bolder",
                                                            "color": "Accent",
                                                            "size": "Medium",
                                                            "maxLines": 3
                                                        },
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "{ResultSnippet}",
                                                            "maxLines": 3,
                                                            "wrap": true
                                                        }
                                                    ],
                                                    "spacing": "Medium"
                                                }
                                            ]
                                        }
                                    ],
                                    "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                                }
                            }
                        }
                    }
                ]
            }

        }

    </script>

</head>

<body onload="renderCard()">
    <h1>Adaptive Cards Data Binding Example</h1>
    <div id="exampleDiv"></div>
</body>

</html>
```

## <a name="see-also"></a>另请参阅

- [创建用于自定义搜索结果的布局](/microsoftsearch/customize-results-layout)
- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview)
