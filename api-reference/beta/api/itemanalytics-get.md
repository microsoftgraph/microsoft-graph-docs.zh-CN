---
author: daspek
description: 获取有关在此资源下发生的视图的 itemAnalytics。
ms.date: 10/06/2017
title: 获取分析结果
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: bb733e8c146d054d88a0b2d24c2f7f114c68522b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975406"
---
# <a name="get-analytics"></a><span data-ttu-id="c6815-103">获取分析结果</span><span class="sxs-lookup"><span data-stu-id="c6815-103">Get analytics</span></span>

<span data-ttu-id="c6815-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6815-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6815-105">获取有关在此资源下发生的视图的 [itemAnalytics][] 。</span><span class="sxs-lookup"><span data-stu-id="c6815-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="c6815-106">**ItemAnalytics** 资源是获取和的活动统计信息的便捷方式 `allTime` `lastSevenDays` 。</span><span class="sxs-lookup"><span data-stu-id="c6815-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="c6815-107">对于自定义时间范围或时间间隔，请使用 [getActivitiesByInterval][] API。</span><span class="sxs-lookup"><span data-stu-id="c6815-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="c6815-108">**注意：\*\*\*\*ItemAnalytics** 资源在所有 [国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="c6815-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="c6815-111">权限</span><span class="sxs-lookup"><span data-stu-id="c6815-111">Permissions</span></span>

<span data-ttu-id="c6815-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6815-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6815-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6815-114">Permission type</span></span>                        | <span data-ttu-id="c6815-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6815-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c6815-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6815-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6815-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6815-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c6815-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6815-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6815-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6815-119">Not supported.</span></span>
|<span data-ttu-id="c6815-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6815-120">Application</span></span>                            | <span data-ttu-id="c6815-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6815-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c6815-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6815-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="c6815-123">示例</span><span class="sxs-lookup"><span data-stu-id="c6815-123">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c6815-124">请求</span><span class="sxs-lookup"><span data-stu-id="c6815-124">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c6815-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6815-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="c6815-126">C#</span><span class="sxs-lookup"><span data-stu-id="c6815-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6815-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6815-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6815-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6815-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6815-129">Java</span><span class="sxs-lookup"><span data-stu-id="c6815-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c6815-130">响应</span><span class="sxs-lookup"><span data-stu-id="c6815-130">Response</span></span>

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


