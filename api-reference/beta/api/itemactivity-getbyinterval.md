---
author: daspek
description: 获取在指定时间间隔内此资源下发生的活动的 itemActivityStats。
ms.date: 10/06/2017
title: 按间隔获取项目活动统计
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: f2c3158fbc7ac8c925bc0bf2556623d01aa7b48d
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123185"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="db7a7-103">按间隔获取项目活动统计</span><span class="sxs-lookup"><span data-stu-id="db7a7-103">Get item activity stats by interval</span></span>

<span data-ttu-id="db7a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db7a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db7a7-105">获取在指定时间间隔内此资源下发生的活动的[itemActivityStats][] 。</span><span class="sxs-lookup"><span data-stu-id="db7a7-105">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="db7a7-106">**注意：\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="db7a7-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="db7a7-107">分析聚合可能不适用于所有操作类型。</span><span class="sxs-lookup"><span data-stu-id="db7a7-107">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="db7a7-109">权限</span><span class="sxs-lookup"><span data-stu-id="db7a7-109">Permissions</span></span>

<span data-ttu-id="db7a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db7a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db7a7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="db7a7-112">Permission type</span></span>                        | <span data-ttu-id="db7a7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db7a7-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="db7a7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db7a7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="db7a7-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db7a7-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="db7a7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db7a7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db7a7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="db7a7-117">Not supported.</span></span>
|<span data-ttu-id="db7a7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="db7a7-118">Application</span></span>                            | <span data-ttu-id="db7a7-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db7a7-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="db7a7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db7a7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="db7a7-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="db7a7-121">Function parameters</span></span>

| <span data-ttu-id="db7a7-122">参数</span><span class="sxs-lookup"><span data-stu-id="db7a7-122">Parameter</span></span>      | <span data-ttu-id="db7a7-123">类型</span><span class="sxs-lookup"><span data-stu-id="db7a7-123">Type</span></span>               | <span data-ttu-id="db7a7-124">说明</span><span class="sxs-lookup"><span data-stu-id="db7a7-124">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="db7a7-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="db7a7-125">startDateTime</span></span>  | <span data-ttu-id="db7a7-126">字符串（时间戳）</span><span class="sxs-lookup"><span data-stu-id="db7a7-126">string (timestamp)</span></span> | <span data-ttu-id="db7a7-127">聚合活动的开始时间。</span><span class="sxs-lookup"><span data-stu-id="db7a7-127">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="db7a7-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="db7a7-128">endDateTime</span></span>    | <span data-ttu-id="db7a7-129">字符串（时间戳）</span><span class="sxs-lookup"><span data-stu-id="db7a7-129">string (timestamp)</span></span> | <span data-ttu-id="db7a7-130">聚合活动的结束时间。</span><span class="sxs-lookup"><span data-stu-id="db7a7-130">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="db7a7-131">interval</span><span class="sxs-lookup"><span data-stu-id="db7a7-131">interval</span></span>       | <span data-ttu-id="db7a7-132">string</span><span class="sxs-lookup"><span data-stu-id="db7a7-132">string</span></span>             | <span data-ttu-id="db7a7-133">聚合间隔。</span><span class="sxs-lookup"><span data-stu-id="db7a7-133">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="db7a7-134">示例</span><span class="sxs-lookup"><span data-stu-id="db7a7-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="db7a7-135">请求</span><span class="sxs-lookup"><span data-stu-id="db7a7-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="db7a7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="db7a7-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="db7a7-137">C#</span><span class="sxs-lookup"><span data-stu-id="db7a7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db7a7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db7a7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db7a7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db7a7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db7a7-140">响应</span><span class="sxs-lookup"><span data-stu-id="db7a7-140">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "startDateTime": "2017-01-01T00:00:00.000Z",
            "endDateTime": "2017-01-02T00:00:00.000Z",
            "delete": {
                "actionCount": 1,
                "actorCount": 1
            },
            "access": {
                "actionCount": 5,
                "actorCount": 3
            }
        },
        {
            "startDateTime": "2017-01-02T00:00:00.000Z",
            "endDateTime": "2017-01-03T00:00:00.000Z",
            "edit": {
                "actionCount": 3,
                "actorCount": 1
            },
            "access": {
                "actionCount": 7,
                "actorCount": 6
            }
        }
    ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval",
  "suppressions": []
}
-->
