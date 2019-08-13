---
author: daspek
description: 获取有关在此资源下发生的视图的 itemAnalytics。
ms.date: 10/06/2017
title: 获取分析结果
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 822664263be00f7a8a2d98a1b0815f693368cf3a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343011"
---
# <a name="get-analytics"></a><span data-ttu-id="779fe-103">获取分析结果</span><span class="sxs-lookup"><span data-stu-id="779fe-103">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="779fe-104">获取有关在此资源下发生的视图的[itemAnalytics][] 。</span><span class="sxs-lookup"><span data-stu-id="779fe-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="779fe-105">**ItemAnalytics**资源是获取`allTime`和的`lastSevenDays`活动统计信息的便捷方式。</span><span class="sxs-lookup"><span data-stu-id="779fe-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="779fe-106">对于自定义时间范围或时间间隔, 请使用[getActivitiesByInterval][] API。</span><span class="sxs-lookup"><span data-stu-id="779fe-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="779fe-107">**注意:\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="779fe-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="779fe-110">权限</span><span class="sxs-lookup"><span data-stu-id="779fe-110">Permissions</span></span>

<span data-ttu-id="779fe-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="779fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="779fe-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="779fe-113">Permission type</span></span>                        | <span data-ttu-id="779fe-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="779fe-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="779fe-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="779fe-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="779fe-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="779fe-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="779fe-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="779fe-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="779fe-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="779fe-118">Not supported.</span></span>
|<span data-ttu-id="779fe-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="779fe-119">Application</span></span>                            | <span data-ttu-id="779fe-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="779fe-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="779fe-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="779fe-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="779fe-122">示例</span><span class="sxs-lookup"><span data-stu-id="779fe-122">Example</span></span>

#### <a name="request"></a><span data-ttu-id="779fe-123">请求</span><span class="sxs-lookup"><span data-stu-id="779fe-123">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="779fe-124">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="779fe-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="779fe-125">C#</span><span class="sxs-lookup"><span data-stu-id="779fe-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="779fe-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="779fe-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="779fe-127">目标-C</span><span class="sxs-lookup"><span data-stu-id="779fe-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="779fe-128">Java</span><span class="sxs-lookup"><span data-stu-id="779fe-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="779fe-129">响应</span><span class="sxs-lookup"><span data-stu-id="779fe-129">Response</span></span>

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
