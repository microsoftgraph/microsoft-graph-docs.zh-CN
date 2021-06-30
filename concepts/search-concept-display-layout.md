---
ms.author: yiwenwang
title: 使用 Microsoft Microsoft 搜索 API Graph呈现显示布局
description: 使用 Microsoft Microsoft 搜索 API Graph以不同方式显示搜索结果。
author: yiwenwang
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 4f58e7b4a303ba6b20b1d70bd765b38d1526bbca
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211166"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-render-display-layout-preview"></a><span data-ttu-id="d0d74-103">使用 Microsoft Microsoft 搜索 中的 Graph API 在预览 (布局) </span><span class="sxs-lookup"><span data-stu-id="d0d74-103">Use the Microsoft Search API in Microsoft Graph to render display layout (preview)</span></span>

<span data-ttu-id="d0d74-104">搜索显示布局或结果类型是导致不同类型的搜索结果以不同方式显示在搜索结果页面中的规则。</span><span class="sxs-lookup"><span data-stu-id="d0d74-104">A search display layout or result type is a rule that causes distinct kinds of search results to be displayed in different ways in search result pages.</span></span> <span data-ttu-id="d0d74-105">它包含以下几个方面：</span><span class="sxs-lookup"><span data-stu-id="d0d74-105">It consists of the following:</span></span> 

- <span data-ttu-id="d0d74-106">要比较每个搜索结果的一个或多个特征或条件，例如搜索结果的结果源或内容类型。</span><span class="sxs-lookup"><span data-stu-id="d0d74-106">One or more characteristics or conditions to compare each search result against, such as the result source or content type of the search result.</span></span>
- <span data-ttu-id="d0d74-p102">用于符合条件的搜索结果的显示模板。显示模板控制满足条件的所有结果在搜索结果页面上的显示和行为方式。</span><span class="sxs-lookup"><span data-stu-id="d0d74-p102">A display template to use for search results that meet the conditions. The display template controls the way in which all results that meet the conditions appear and behave on a search results page.</span></span> 

<span data-ttu-id="d0d74-109">Microsoft Graph 搜索 API 提供基于自适应卡片的可[呈现响应](https://adaptivecards.io/)。</span><span class="sxs-lookup"><span data-stu-id="d0d74-109">The Microsoft Graph Search API provides a renderable response based on [Adaptive Cards](https://adaptivecards.io/).</span></span> <span data-ttu-id="d0d74-110">通过使用自适应 [卡片模板](https://adaptivecards.io/designer)，客户端可以在不同的画布中呈现不同的搜索结果。</span><span class="sxs-lookup"><span data-stu-id="d0d74-110">By using the [Adaptive Card template](https://adaptivecards.io/designer), clients can render different search result in different canvases.</span></span>

<span data-ttu-id="d0d74-111">客户可以在网站中自定义其[Microsoft 365 管理中心。](https://admin.microsoft.com/Adminportal/Home#/MicrosoftSearch/resulttypes)</span><span class="sxs-lookup"><span data-stu-id="d0d74-111">Customers can customize their search result type in the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home#/MicrosoftSearch/resulttypes).</span></span>

## <a name="request-example"></a><span data-ttu-id="d0d74-112">请求示例</span><span class="sxs-lookup"><span data-stu-id="d0d74-112">Request example</span></span>

<span data-ttu-id="d0d74-113">以下示例演示如何在请求合约中将 **enableResultTemplate** 属性设置为 ，获取用于呈现搜索结果的显示布局或 `true` 结果模板。</span><span class="sxs-lookup"><span data-stu-id="d0d74-113">The following example shows how to get the display layouts or result templates for rendering the search results by setting the **enableResultTemplate** property to `true` in the request contract.</span></span>

<span data-ttu-id="d0d74-114">重新点击显示三个搜索命中，其中两个与 **resultTemplateId** 1603900360618_5XCBK2OXG相关，另一个与 **resultTemplateId** 1603900360618_5XCBK2OXP。</span><span class="sxs-lookup"><span data-stu-id="d0d74-114">The reponse shows three search hits, two of them related, with the **resultTemplateId** 1603900360618_5XCBK2OXG, and the other one with the **resultTemplateId** 1603900360618_5XCBK2OXP.</span></span> <span data-ttu-id="d0d74-115">这些 ID 与包含在响应协定中的 **resultTemplates** 字典中的两个显示布局的键之一匹配。</span><span class="sxs-lookup"><span data-stu-id="d0d74-115">These IDs match with one of the keys of the two display layouts contained in the **resultTemplates** dictionary that's included within the response contract.</span></span> <span data-ttu-id="d0d74-116">使用结果模板 ID，可以确定用于呈现每个搜索结果的显示布局。</span><span class="sxs-lookup"><span data-stu-id="d0d74-116">Using the result template IDs, you can determine which display layout to use to render each search result.</span></span>

### <a name="request"></a><span data-ttu-id="d0d74-117">请求</span><span class="sxs-lookup"><span data-stu-id="d0d74-117">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="d0d74-118">响应</span><span class="sxs-lookup"><span data-stu-id="d0d74-118">Response</span></span>


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

## <a name="web-component-example"></a><span data-ttu-id="d0d74-119">Web 组件示例</span><span class="sxs-lookup"><span data-stu-id="d0d74-119">Web component example</span></span>

<span data-ttu-id="d0d74-120">以下示例演示如何使用自适应卡片模板来呈现搜索结果。</span><span class="sxs-lookup"><span data-stu-id="d0d74-120">The following example shows how to use Adaptive Card templating to render search results.</span></span>

> [!IMPORTANT] 
> 
> <span data-ttu-id="d0d74-121">此示例使用早于 **2020** 年 5 月版本的自适应卡片模板版本。</span><span class="sxs-lookup"><span data-stu-id="d0d74-121">This example uses a version of Adaptive Card templating earlier than the **May 2020 release**.</span></span> <span data-ttu-id="d0d74-122">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="d0d74-122">For more details, see:</span></span>
> - [<span data-ttu-id="d0d74-123">自适应卡片模板</span><span class="sxs-lookup"><span data-stu-id="d0d74-123">Adaptive Card templating</span></span>](/adaptive-cards/templating/)
> - [<span data-ttu-id="d0d74-124">自适应卡片模板 SDK</span><span class="sxs-lookup"><span data-stu-id="d0d74-124">Adaptive Card templating SDK</span></span>](/adaptive-cards/templating/sdk)


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

## <a name="next-steps"></a><span data-ttu-id="d0d74-125">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d0d74-125">Next steps</span></span>

- [<span data-ttu-id="d0d74-126">使用 Microsoft 搜索 API</span><span class="sxs-lookup"><span data-stu-id="d0d74-126">Use the Microsoft Search API</span></span>](/graph/api/resources/search-api-overview)
