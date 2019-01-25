---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 按间隔中获取项活动状态
localization_priority: Normal
ms.openlocfilehash: f9601538d825efe346ab57fdbecd6c74dc9978d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516453"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="b90eb-102">按间隔中获取项活动状态</span><span class="sxs-lookup"><span data-stu-id="b90eb-102">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b90eb-103">[ItemActivityStats][]获得的指定的时间间隔内发生下此资源的活动。</span><span class="sxs-lookup"><span data-stu-id="b90eb-103">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="b90eb-104">**注意：\*\*\*\*ItemAnalytics**资源尚不可用所有[国家/地区的部署](/graph/deployments)中。</span><span class="sxs-lookup"><span data-stu-id="b90eb-104">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="b90eb-105">分析聚合可能不可用的所有操作类型。</span><span class="sxs-lookup"><span data-stu-id="b90eb-105">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="b90eb-107">权限</span><span class="sxs-lookup"><span data-stu-id="b90eb-107">Permissions</span></span>

<span data-ttu-id="b90eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b90eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b90eb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b90eb-110">Permission type</span></span>                        | <span data-ttu-id="b90eb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b90eb-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="b90eb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b90eb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b90eb-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b90eb-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="b90eb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b90eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b90eb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b90eb-115">Not supported.</span></span>
|<span data-ttu-id="b90eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b90eb-116">Application</span></span>                            | <span data-ttu-id="b90eb-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b90eb-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b90eb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b90eb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="b90eb-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="b90eb-119">Function parameters</span></span>

| <span data-ttu-id="b90eb-120">参数</span><span class="sxs-lookup"><span data-stu-id="b90eb-120">Parameter</span></span>      | <span data-ttu-id="b90eb-121">类型</span><span class="sxs-lookup"><span data-stu-id="b90eb-121">Type</span></span>               | <span data-ttu-id="b90eb-122">说明</span><span class="sxs-lookup"><span data-stu-id="b90eb-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="b90eb-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b90eb-123">startDateTime</span></span>  | <span data-ttu-id="b90eb-124">字符串 （时间戳）</span><span class="sxs-lookup"><span data-stu-id="b90eb-124">string (timestamp)</span></span> | <span data-ttu-id="b90eb-125">聚合活动的开始时间。</span><span class="sxs-lookup"><span data-stu-id="b90eb-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="b90eb-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b90eb-126">endDateTime</span></span>    | <span data-ttu-id="b90eb-127">字符串 （时间戳）</span><span class="sxs-lookup"><span data-stu-id="b90eb-127">string (timestamp)</span></span> | <span data-ttu-id="b90eb-128">聚合活动哪些结束时间。</span><span class="sxs-lookup"><span data-stu-id="b90eb-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="b90eb-129">interval</span><span class="sxs-lookup"><span data-stu-id="b90eb-129">interval</span></span>       | <span data-ttu-id="b90eb-130">string</span><span class="sxs-lookup"><span data-stu-id="b90eb-130">string</span></span>             | <span data-ttu-id="b90eb-131">聚合时间间隔。</span><span class="sxs-lookup"><span data-stu-id="b90eb-131">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="b90eb-132">示例</span><span class="sxs-lookup"><span data-stu-id="b90eb-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b90eb-133">请求</span><span class="sxs-lookup"><span data-stu-id="b90eb-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="b90eb-134">响应</span><span class="sxs-lookup"><span data-stu-id="b90eb-134">Response</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/itemactivity-getbyinterval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
