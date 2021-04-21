---
title: searchEntity： query
description: 运行请求正文中指定的查询。 响应中提供了搜索结果。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 8194b23ede8856f0237b179aa4d50a5ce0c1ebc9
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920108"
---
# <a name="searchentity-query"></a><span data-ttu-id="0312d-104">searchEntity： query</span><span class="sxs-lookup"><span data-stu-id="0312d-104">searchEntity: query</span></span>

<span data-ttu-id="0312d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0312d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0312d-106">运行请求正文中指定的查询。</span><span class="sxs-lookup"><span data-stu-id="0312d-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="0312d-107">响应中提供了搜索结果。</span><span class="sxs-lookup"><span data-stu-id="0312d-107">Search results are provided in the response.</span></span>


## <a name="permissions"></a><span data-ttu-id="0312d-108">权限</span><span class="sxs-lookup"><span data-stu-id="0312d-108">Permissions</span></span>

<span data-ttu-id="0312d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0312d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="0312d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0312d-111">Permission type</span></span>                        | <span data-ttu-id="0312d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0312d-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0312d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0312d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0312d-114">Mail.Read、Calendars.Read、Files.Read.All、Sites.Read.All、ExternalItem.Read.All</span><span class="sxs-lookup"><span data-stu-id="0312d-114">Mail.Read, Calendars.Read, Files.Read.All, Sites.Read.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="0312d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0312d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0312d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0312d-116">Not supported.</span></span> |
| <span data-ttu-id="0312d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0312d-117">Application</span></span>                            | <span data-ttu-id="0312d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0312d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0312d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0312d-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="0312d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0312d-120">Request headers</span></span>

| <span data-ttu-id="0312d-121">名称</span><span class="sxs-lookup"><span data-stu-id="0312d-121">Name</span></span>          | <span data-ttu-id="0312d-122">说明</span><span class="sxs-lookup"><span data-stu-id="0312d-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0312d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0312d-123">Authorization</span></span> | <span data-ttu-id="0312d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0312d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0312d-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="0312d-126">Content-type</span></span> | <span data-ttu-id="0312d-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0312d-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0312d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0312d-129">Request body</span></span>

<span data-ttu-id="0312d-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0312d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0312d-131">参数</span><span class="sxs-lookup"><span data-stu-id="0312d-131">Parameter</span></span>    | <span data-ttu-id="0312d-132">类型</span><span class="sxs-lookup"><span data-stu-id="0312d-132">Type</span></span>        | <span data-ttu-id="0312d-133">说明</span><span class="sxs-lookup"><span data-stu-id="0312d-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0312d-134">requests</span><span class="sxs-lookup"><span data-stu-id="0312d-134">requests</span></span>|<span data-ttu-id="0312d-135">[searchRequest](../resources/searchrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0312d-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="0312d-136">一个或多个搜索请求的集合，每个搜索请求的格式都为 JSON blob。</span><span class="sxs-lookup"><span data-stu-id="0312d-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="0312d-137">每个 JSON blob 都包含响应中预期的资源类型、基础源、分页参数、请求的字段和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="0312d-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="0312d-138">请注意搜索 [实体](../resources/search-api-overview.md#known-limitations) 类型的特定组合以及排序或聚合搜索结果的已知限制。</span><span class="sxs-lookup"><span data-stu-id="0312d-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |

## <a name="response"></a><span data-ttu-id="0312d-139">响应</span><span class="sxs-lookup"><span data-stu-id="0312d-139">Response</span></span>

<span data-ttu-id="0312d-140">如果成功，此方法在响应正文中返回 响应代码和 `HTTP 200 OK` [searchResponse](../resources/searchresponse.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="0312d-140">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="0312d-141">示例</span><span class="sxs-lookup"><span data-stu-id="0312d-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0312d-142">请求</span><span class="sxs-lookup"><span data-stu-id="0312d-142">Request</span></span>

<span data-ttu-id="0312d-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0312d-143">The following is an example of the request.</span></span>

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0312d-144">响应</span><span class="sxs-lookup"><span data-stu-id="0312d-144">Response</span></span>

<span data-ttu-id="0312d-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0312d-145">The following is an example of the response.</span></span>

> <span data-ttu-id="0312d-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0312d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.searchResponse",
  "isCollection": true
} -->

```HTTP
HTTP/1.1 200 OK
Content-type: application/json
```

```json
{
    "value": [
        {
            "searchTerms": [
                "searchTerms-value"
            ],
            "hitsContainers": [
                {
                    "hits": [
                        {
                            "hitId": "AAMkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZABGAAAAAACsLZF5BeQoRLYm4UlvnOXZBwCav2PZy/7/R52ssyzmS9f0AAAAAAEMAACav2PZy/7/R52ssyzmS9f0AABM0pr/AAA=",
                            "rank": 1,
                            "summary": "...Identity Protection Weekly Digest <c0>Contoso</c0> New risky users detected <https://azure.microsoft.com/email/?destination=https%3A%2F%2Fportal.azure.com%2Fcontoso.com%23blade%2FMicrosoft_AAD_IAM%2FIdentityProtectionMenuBlade%2FRiskyUsers%2F...",
                            "resource": {
                                "@odata.type": "#microsoft.graph.message",
                                "createdDateTime": "2020-11-17T16:02:34Z",
                                "lastModifiedDateTime": "2020-11-17T16:02:37Z",
                                "changeKey": "CQAAAA==",
                                "receivedDateTime": "2020-11-17T16:02:34Z",
                                "sentDateTime": "2020-11-17T16:02:27Z",
                                "hasAttachments": false,
                                "internetMessageId": "<1e506769-c6da-4f44-bb54-6ba1bd59d300@az.northcentralus.production.microsoft.com>",
                                "subject": "Azure AD Identity Protection Weekly Digest",
                                "bodyPreview": "...Identity Protection Weekly Digest Contoso New risky users detected <https://azure.microsoft.com/email/?destination=https%3A%2F%2Fportal.azure.com%2Fcontoso.com%23blade%2FMicrosoft_AAD_IAM%2FIdentityProtectionMenuBlade%2FRiskyUsers%2F...",
                                "importance": "normal",
                                "parentFolderId": "AQMkADdmODdhN2NjAC0zMGVmLTQwYjctYjA2MS1mYWU5MjhjOGJkYWQALgAAA6wtkXkF5ChEtibhSW+c5dkBAJq/Y9nL/v9HnayzLOZL1/QAAAIBDAAAAA==",
                                "conversationId": "AAQkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZAAQAKQ6a/rTEmVCtGMTER183jw=",
                                "isRead": false,
                                "isDraft": false,
                                "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZABGAAAAAACsLZF5BeQoRLYm4UlvnOXZBwCav2PZy%2F7%2FR52ssyzmS9f0AAAAAAEMAACav2PZy%2F7%2FR52ssyzmS9f0AABM0pr%2FAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
                                "inferenceClassification": "focused",
                                "replyTo": [
                                    {
                                        "emailAddress": {
                                            "name": "MOD Administrator"
                                        }
                                    }
                                ],
                                "sender": {
                                    "emailAddress": {
                                        "name": "Microsoft Azure",
                                        "address": "azure-noreply@contoso.com"
                                    }
                                },
                                "from": {
                                    "emailAddress": {
                                        "name": "Microsoft Azure",
                                        "address": "azure-noreply@contoso.com"
                                    }
                                }
                            }
                        }
                    ],
                    "total": 47,
                    "moreResultsAvailable": true
                }
            ]
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="0312d-148">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0312d-148">See also</span></span>
- <span data-ttu-id="0312d-149">搜索 [邮件](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="0312d-149">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="0312d-150">搜索 [日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="0312d-150">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="0312d-151">在 SharePoint 和 OneDrive 中搜索 ([文件、列表和网站) ](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="0312d-151">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="0312d-152">使用 [Graph 连接器 (搜索) ](/graph/search-concept-custom-types) 类型</span><span class="sxs-lookup"><span data-stu-id="0312d-152">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


