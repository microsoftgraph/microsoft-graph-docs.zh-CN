---
author: daspek
description: 获取在指定时间间隔内此资源下发生的活动的 itemActivityStats。
ms.date: 10/06/2017
title: 按间隔获取项目活动统计
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 6d1f7a3b4e6a326f107a0d0ff33db59ed73f2794
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979104"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="92ec7-103">按间隔获取项目活动统计</span><span class="sxs-lookup"><span data-stu-id="92ec7-103">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92ec7-104">获取在指定时间间隔内此资源下发生的活动的[itemActivityStats][] 。</span><span class="sxs-lookup"><span data-stu-id="92ec7-104">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="92ec7-105">**注意:\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="92ec7-105">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="92ec7-106">分析聚合可能不适用于所有操作类型。</span><span class="sxs-lookup"><span data-stu-id="92ec7-106">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="92ec7-108">权限</span><span class="sxs-lookup"><span data-stu-id="92ec7-108">Permissions</span></span>

<span data-ttu-id="92ec7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92ec7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ec7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="92ec7-111">Permission type</span></span>                        | <span data-ttu-id="92ec7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92ec7-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="92ec7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92ec7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="92ec7-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ec7-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="92ec7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92ec7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92ec7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="92ec7-116">Not supported.</span></span>
|<span data-ttu-id="92ec7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="92ec7-117">Application</span></span>                            | <span data-ttu-id="92ec7-118">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ec7-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="92ec7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92ec7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="92ec7-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="92ec7-120">Function parameters</span></span>

| <span data-ttu-id="92ec7-121">参数</span><span class="sxs-lookup"><span data-stu-id="92ec7-121">Parameter</span></span>      | <span data-ttu-id="92ec7-122">类型</span><span class="sxs-lookup"><span data-stu-id="92ec7-122">Type</span></span>               | <span data-ttu-id="92ec7-123">说明</span><span class="sxs-lookup"><span data-stu-id="92ec7-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="92ec7-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="92ec7-124">startDateTime</span></span>  | <span data-ttu-id="92ec7-125">字符串 (时间戳)</span><span class="sxs-lookup"><span data-stu-id="92ec7-125">string (timestamp)</span></span> | <span data-ttu-id="92ec7-126">聚合活动的开始时间。</span><span class="sxs-lookup"><span data-stu-id="92ec7-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="92ec7-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="92ec7-127">endDateTime</span></span>    | <span data-ttu-id="92ec7-128">字符串 (时间戳)</span><span class="sxs-lookup"><span data-stu-id="92ec7-128">string (timestamp)</span></span> | <span data-ttu-id="92ec7-129">聚合活动的结束时间。</span><span class="sxs-lookup"><span data-stu-id="92ec7-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="92ec7-130">interval</span><span class="sxs-lookup"><span data-stu-id="92ec7-130">interval</span></span>       | <span data-ttu-id="92ec7-131">string</span><span class="sxs-lookup"><span data-stu-id="92ec7-131">string</span></span>             | <span data-ttu-id="92ec7-132">聚合间隔。</span><span class="sxs-lookup"><span data-stu-id="92ec7-132">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="92ec7-133">示例</span><span class="sxs-lookup"><span data-stu-id="92ec7-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="92ec7-134">请求</span><span class="sxs-lookup"><span data-stu-id="92ec7-134">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="92ec7-135">响应</span><span class="sxs-lookup"><span data-stu-id="92ec7-135">Response</span></span>

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
