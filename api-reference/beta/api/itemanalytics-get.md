---
author: daspek
description: 获取有关在此资源下发生的视图的 itemAnalytics。
ms.date: 10/06/2017
title: 获取分析结果
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 3b8c423037acd0af5c82bc350f8e859d00c4069a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457270"
---
# <a name="get-analytics"></a><span data-ttu-id="d252b-103">获取分析结果</span><span class="sxs-lookup"><span data-stu-id="d252b-103">Get analytics</span></span>

<span data-ttu-id="d252b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d252b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d252b-105">获取有关在此资源下发生的视图的[itemAnalytics][] 。</span><span class="sxs-lookup"><span data-stu-id="d252b-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="d252b-106">**ItemAnalytics**资源是获取`allTime`和的`lastSevenDays`活动统计信息的便捷方式。</span><span class="sxs-lookup"><span data-stu-id="d252b-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="d252b-107">对于自定义时间范围或时间间隔，请使用[getActivitiesByInterval][] API。</span><span class="sxs-lookup"><span data-stu-id="d252b-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="d252b-108">**注意：\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="d252b-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="d252b-111">权限</span><span class="sxs-lookup"><span data-stu-id="d252b-111">Permissions</span></span>

<span data-ttu-id="d252b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d252b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d252b-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="d252b-114">Permission type</span></span>                        | <span data-ttu-id="d252b-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d252b-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d252b-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d252b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d252b-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d252b-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="d252b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d252b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d252b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d252b-119">Not supported.</span></span>
|<span data-ttu-id="d252b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d252b-120">Application</span></span>                            | <span data-ttu-id="d252b-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d252b-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d252b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d252b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="d252b-123">示例</span><span class="sxs-lookup"><span data-stu-id="d252b-123">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d252b-124">请求</span><span class="sxs-lookup"><span data-stu-id="d252b-124">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d252b-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="d252b-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="d252b-126">C#</span><span class="sxs-lookup"><span data-stu-id="d252b-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d252b-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d252b-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d252b-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d252b-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d252b-129">响应</span><span class="sxs-lookup"><span data-stu-id="d252b-129">Response</span></span>

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
