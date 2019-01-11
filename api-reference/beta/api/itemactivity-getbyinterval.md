---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 按间隔中获取项活动状态
localization_priority: Normal
ms.openlocfilehash: 7ca0e4e4767073d37ebeabbab10e1f50ce323599
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826864"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="0ff01-102">按间隔中获取项活动状态</span><span class="sxs-lookup"><span data-stu-id="0ff01-102">Get item activity stats by interval</span></span>

> <span data-ttu-id="0ff01-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ff01-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ff01-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ff01-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ff01-105">[ItemActivityStats][]获得的指定的时间间隔内发生下此资源的活动。</span><span class="sxs-lookup"><span data-stu-id="0ff01-105">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="0ff01-106">**注意：\*\*\*\*ItemAnalytics**资源尚不可用所有[国家/地区的部署](/graph/deployments)中。</span><span class="sxs-lookup"><span data-stu-id="0ff01-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="0ff01-107">分析聚合可能不可用的所有操作类型。</span><span class="sxs-lookup"><span data-stu-id="0ff01-107">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="0ff01-109">权限</span><span class="sxs-lookup"><span data-stu-id="0ff01-109">Permissions</span></span>

<span data-ttu-id="0ff01-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ff01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ff01-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ff01-112">Permission type</span></span>                        | <span data-ttu-id="0ff01-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ff01-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="0ff01-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ff01-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ff01-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff01-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="0ff01-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ff01-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ff01-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ff01-117">Not supported.</span></span>
|<span data-ttu-id="0ff01-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ff01-118">Application</span></span>                            | <span data-ttu-id="0ff01-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff01-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="0ff01-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ff01-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="0ff01-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="0ff01-121">Function parameters</span></span>

| <span data-ttu-id="0ff01-122">参数</span><span class="sxs-lookup"><span data-stu-id="0ff01-122">Parameter</span></span>      | <span data-ttu-id="0ff01-123">类型</span><span class="sxs-lookup"><span data-stu-id="0ff01-123">Type</span></span>               | <span data-ttu-id="0ff01-124">说明</span><span class="sxs-lookup"><span data-stu-id="0ff01-124">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="0ff01-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0ff01-125">startDateTime</span></span>  | <span data-ttu-id="0ff01-126">字符串 （时间戳）</span><span class="sxs-lookup"><span data-stu-id="0ff01-126">string (timestamp)</span></span> | <span data-ttu-id="0ff01-127">聚合活动的开始时间。</span><span class="sxs-lookup"><span data-stu-id="0ff01-127">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="0ff01-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0ff01-128">endDateTime</span></span>    | <span data-ttu-id="0ff01-129">字符串 （时间戳）</span><span class="sxs-lookup"><span data-stu-id="0ff01-129">string (timestamp)</span></span> | <span data-ttu-id="0ff01-130">聚合活动哪些结束时间。</span><span class="sxs-lookup"><span data-stu-id="0ff01-130">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="0ff01-131">interval</span><span class="sxs-lookup"><span data-stu-id="0ff01-131">interval</span></span>       | <span data-ttu-id="0ff01-132">string</span><span class="sxs-lookup"><span data-stu-id="0ff01-132">string</span></span>             | <span data-ttu-id="0ff01-133">聚合时间间隔。</span><span class="sxs-lookup"><span data-stu-id="0ff01-133">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="0ff01-134">示例</span><span class="sxs-lookup"><span data-stu-id="0ff01-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0ff01-135">请求</span><span class="sxs-lookup"><span data-stu-id="0ff01-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="0ff01-136">响应</span><span class="sxs-lookup"><span data-stu-id="0ff01-136">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval"
} -->
