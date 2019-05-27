---
author: daspek
ms.author: dspektor
title: 获取 itemAnalytics
description: 获取有关在此资源下发生的视图的 itemAnalytics。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3923237cd608207f0c06f4acd3bb241b2808605d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461606"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="d5012-103">获取 itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="d5012-103">Get itemAnalytics</span></span>

<span data-ttu-id="d5012-104">获取有关在此资源下发生的视图的[itemAnalytics][] 。</span><span class="sxs-lookup"><span data-stu-id="d5012-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="d5012-105">**ItemAnalytics**资源是获取`allTime`和的`lastSevenDays`活动统计信息的便捷方式。</span><span class="sxs-lookup"><span data-stu-id="d5012-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="d5012-106">对于自定义时间范围或时间间隔, 请使用[getActivitiesByInterval][] API。</span><span class="sxs-lookup"><span data-stu-id="d5012-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="d5012-107">**注意:\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="d5012-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="d5012-110">权限</span><span class="sxs-lookup"><span data-stu-id="d5012-110">Permissions</span></span>

<span data-ttu-id="d5012-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5012-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5012-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5012-113">Permission type</span></span>                        | <span data-ttu-id="d5012-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5012-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d5012-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5012-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5012-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5012-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="d5012-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5012-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5012-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5012-118">Not supported.</span></span>
|<span data-ttu-id="d5012-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5012-119">Application</span></span>                            | <span data-ttu-id="d5012-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5012-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d5012-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5012-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d5012-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d5012-122">Optional query parameters</span></span>
<span data-ttu-id="d5012-123">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d5012-123">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5012-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5012-124">Request headers</span></span>

| <span data-ttu-id="d5012-125">名称</span><span class="sxs-lookup"><span data-stu-id="d5012-125">Name</span></span>      |<span data-ttu-id="d5012-126">说明</span><span class="sxs-lookup"><span data-stu-id="d5012-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5012-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5012-127">Authorization</span></span>  | <span data-ttu-id="d5012-128">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="d5012-128">Bearer {code}.</span></span> <span data-ttu-id="d5012-129">必需。</span><span class="sxs-lookup"><span data-stu-id="d5012-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5012-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5012-130">Request body</span></span>

<span data-ttu-id="d5012-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5012-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5012-132">响应</span><span class="sxs-lookup"><span data-stu-id="d5012-132">Response</span></span> 

<span data-ttu-id="d5012-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[itemAnalytics][]对象集合。</span><span class="sxs-lookup"><span data-stu-id="d5012-133">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="d5012-134">示例</span><span class="sxs-lookup"><span data-stu-id="d5012-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5012-135">请求</span><span class="sxs-lookup"><span data-stu-id="d5012-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

### <a name="response"></a><span data-ttu-id="d5012-136">响应</span><span class="sxs-lookup"><span data-stu-id="d5012-136">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d5012-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d5012-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d5012-138">C#</span><span class="sxs-lookup"><span data-stu-id="d5012-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-analytics-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5012-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5012-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-analytics-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
    "Error: /api-reference/v1.0/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
  ]
}
-->
