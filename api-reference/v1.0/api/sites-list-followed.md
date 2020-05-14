---
author: learafa
description: 已登录用户的关注网站列表。
title: 关注网站列表
localization_priority: Normal
ms.prod: SharePoint
doc_type: apiPageType
ms.openlocfilehash: c08def6b72869cdc1886a71d1083dfdef51dbebd
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44052316"
---
# <a name="list-followed-sites"></a><span data-ttu-id="c97d7-103">关注网站列表</span><span class="sxs-lookup"><span data-stu-id="c97d7-103">List followed sites</span></span>

<span data-ttu-id="c97d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c97d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c97d7-105">列出已登录用户的后续[网站](../resources/site.md)。</span><span class="sxs-lookup"><span data-stu-id="c97d7-105">List the [sites](../resources/site.md) that have been followed by the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c97d7-106">权限</span><span class="sxs-lookup"><span data-stu-id="c97d7-106">Permissions</span></span>

<span data-ttu-id="c97d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c97d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c97d7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c97d7-109">Permission type</span></span>      | <span data-ttu-id="c97d7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c97d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c97d7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c97d7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c97d7-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c97d7-112">Sites.Read.All, Sites.ReadWrite.All</span></span>  |
|<span data-ttu-id="c97d7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c97d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c97d7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c97d7-114">Not supported.</span></span>    |
|<span data-ttu-id="c97d7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c97d7-115">Application</span></span> | <span data-ttu-id="c97d7-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c97d7-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c97d7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c97d7-117">HTTP request</span></span>

<span data-ttu-id="c97d7-118">此方法只能通过 OneDrive for Business 访问。</span><span class="sxs-lookup"><span data-stu-id="c97d7-118">This method is accessible only through OneDrive for Business.</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/followedSites
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c97d7-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c97d7-119">Optional query parameters</span></span>
<span data-ttu-id="c97d7-120">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c97d7-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c97d7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c97d7-121">Request headers</span></span>

| <span data-ttu-id="c97d7-122">名称</span><span class="sxs-lookup"><span data-stu-id="c97d7-122">Name</span></span>      |<span data-ttu-id="c97d7-123">说明</span><span class="sxs-lookup"><span data-stu-id="c97d7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c97d7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c97d7-124">Authorization</span></span>  | <span data-ttu-id="c97d7-125">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="c97d7-125">Bearer {code}.</span></span> <span data-ttu-id="c97d7-126">必需。</span><span class="sxs-lookup"><span data-stu-id="c97d7-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c97d7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c97d7-127">Request Body</span></span>

<span data-ttu-id="c97d7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c97d7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c97d7-129">响应</span><span class="sxs-lookup"><span data-stu-id="c97d7-129">Response</span></span>

<span data-ttu-id="c97d7-130">此方法返回用户正在关注的[网站](../resources/site.md)资源的集合。</span><span class="sxs-lookup"><span data-stu-id="c97d7-130">This method returns a collection of [site](../resources/site.md) resources that the user is following.</span></span>
<span data-ttu-id="c97d7-131">如果找不到任何网站，则返回一个空集合。</span><span class="sxs-lookup"><span data-stu-id="c97d7-131">If no sites were found, an empty collection is returned.</span></span>

## <a name="example"></a><span data-ttu-id="c97d7-132">示例</span><span class="sxs-lookup"><span data-stu-id="c97d7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c97d7-133">请求</span><span class="sxs-lookup"><span data-stu-id="c97d7-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c97d7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c97d7-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
POST /me/followedSites
```
# <a name="javascript"></a>[<span data-ttu-id="c97d7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c97d7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c97d7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c97d7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c97d7-137">响应</span><span class="sxs-lookup"><span data-stu-id="c97d7-137">Response</span></span>
<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.site)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        {
            "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
            "displayName": "OneDrive Team Site",
            "webUrl": "https://contoso.sharepoint.com/teams/1drvteam",
            "sharepointIds": {
                "listItemId": "1",
                "siteId": "2C712604-1370-44E7-A1F5-426573FDA80A",
                "siteUrl": "https://contoso.sharepoint.com/teams/1drvteam",
                "webId": "2D2244C3-251A-49EA-93A8-39E1C3A060FE"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        },
        {
            "id": "contoso.sharepoint.com,1C712604-1370-44E7-A1F5-426573FDA80A,1D2244C3-251A-49EA-93A8-39E1C3A060FE",
            "displayName": "OneDrive Team Site1",
            "webUrl": "https://contoso.sharepoint.com/teams/2drvteam",
            "sharepointIds": {
                "listItemId": "1",
                "siteId": "1C712604-1370-44E7-A1F5-426573FDA80A",
                "siteUrl": "https://contoso.sharepoint.com/teams/2drvteam",
                "webId": "1D2244C3-251A-49EA-93A8-39E1C3A060FE"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the sites a user is following.",
  "keywords": "site,onedrive.site,list followed sites, followedSites",
  "section": "documentation",
  "tocPath": "Sites/List followed sites",
  "suppressions": [
  ]
}
-->
