---
author: daspek
description: 获取有关在此资源下发生的视图的 itemAnalytics。
ms.date: 10/06/2017
title: 获取分析结果
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 9dc2fa1360c488b802510395a18364fe45c4c50c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726191"
---
# <a name="get-analytics"></a><span data-ttu-id="b7c41-103">获取分析结果</span><span class="sxs-lookup"><span data-stu-id="b7c41-103">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7c41-104">获取有关在此资源下发生的视图的[itemAnalytics][] 。</span><span class="sxs-lookup"><span data-stu-id="b7c41-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="b7c41-105">**ItemAnalytics**资源是获取`allTime`和的`lastSevenDays`活动统计信息的便捷方式。</span><span class="sxs-lookup"><span data-stu-id="b7c41-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="b7c41-106">对于自定义时间范围或时间间隔, 请使用[getActivitiesByInterval][] API。</span><span class="sxs-lookup"><span data-stu-id="b7c41-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="b7c41-107">**注意:\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="b7c41-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="b7c41-110">权限</span><span class="sxs-lookup"><span data-stu-id="b7c41-110">Permissions</span></span>

<span data-ttu-id="b7c41-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7c41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7c41-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7c41-113">Permission type</span></span>                        | <span data-ttu-id="b7c41-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7c41-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="b7c41-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7c41-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7c41-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7c41-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="b7c41-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7c41-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7c41-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7c41-118">Not supported.</span></span>
|<span data-ttu-id="b7c41-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7c41-119">Application</span></span>                            | <span data-ttu-id="b7c41-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7c41-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b7c41-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7c41-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="b7c41-122">示例</span><span class="sxs-lookup"><span data-stu-id="b7c41-122">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b7c41-123">请求</span><span class="sxs-lookup"><span data-stu-id="b7c41-123">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b7c41-124">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b7c41-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7c41-125">C#</span><span class="sxs-lookup"><span data-stu-id="b7c41-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7c41-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7c41-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7c41-127">目标-C</span><span class="sxs-lookup"><span data-stu-id="b7c41-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b7c41-128">响应</span><span class="sxs-lookup"><span data-stu-id="b7c41-128">Response</span></span>

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
