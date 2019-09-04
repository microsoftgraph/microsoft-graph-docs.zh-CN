---
author: daspek
ms.author: dspektor
title: 获取 itemAnalytics
description: 获取有关在此资源下发生的视图的 itemAnalytics。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c71a86b2ee8fcaa12c17e5b7428480fe12dd203d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730279"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="8c336-103">获取 itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="8c336-103">Get itemAnalytics</span></span>

<span data-ttu-id="8c336-104">获取有关在此资源下发生的视图的[itemAnalytics][] 。</span><span class="sxs-lookup"><span data-stu-id="8c336-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="8c336-105">**ItemAnalytics**资源是获取`allTime`和的`lastSevenDays`活动统计信息的便捷方式。</span><span class="sxs-lookup"><span data-stu-id="8c336-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="8c336-106">对于自定义时间范围或时间间隔, 请使用[getActivitiesByInterval][] API。</span><span class="sxs-lookup"><span data-stu-id="8c336-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="8c336-107">**注意:\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="8c336-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="8c336-110">权限</span><span class="sxs-lookup"><span data-stu-id="8c336-110">Permissions</span></span>

<span data-ttu-id="8c336-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c336-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c336-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c336-113">Permission type</span></span>                        | <span data-ttu-id="8c336-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c336-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="8c336-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c336-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c336-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c336-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="8c336-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c336-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c336-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c336-118">Not supported.</span></span>
|<span data-ttu-id="8c336-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c336-119">Application</span></span>                            | <span data-ttu-id="8c336-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c336-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="8c336-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c336-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c336-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8c336-122">Optional query parameters</span></span>
<span data-ttu-id="8c336-123">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8c336-123">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c336-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c336-124">Request headers</span></span>

| <span data-ttu-id="8c336-125">名称</span><span class="sxs-lookup"><span data-stu-id="8c336-125">Name</span></span>      |<span data-ttu-id="8c336-126">说明</span><span class="sxs-lookup"><span data-stu-id="8c336-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c336-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c336-127">Authorization</span></span>  | <span data-ttu-id="8c336-128">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="8c336-128">Bearer {code}.</span></span> <span data-ttu-id="8c336-129">必需。</span><span class="sxs-lookup"><span data-stu-id="8c336-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c336-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c336-130">Request body</span></span>

<span data-ttu-id="8c336-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c336-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c336-132">响应</span><span class="sxs-lookup"><span data-stu-id="8c336-132">Response</span></span> 

<span data-ttu-id="8c336-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[itemAnalytics][]对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c336-133">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="8c336-134">示例</span><span class="sxs-lookup"><span data-stu-id="8c336-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c336-135">请求</span><span class="sxs-lookup"><span data-stu-id="8c336-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8c336-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8c336-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c336-137">C#</span><span class="sxs-lookup"><span data-stu-id="8c336-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c336-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c336-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c336-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="8c336-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8c336-140">Java</span><span class="sxs-lookup"><span data-stu-id="8c336-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c336-141">响应</span><span class="sxs-lookup"><span data-stu-id="8c336-141">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
  ]
}
-->
