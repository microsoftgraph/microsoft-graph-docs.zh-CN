---
author: daspek
ms.author: dspektor
title: 按间隔获取项目活动统计
description: 获取在指定时间间隔内发生在此资源上的活动的 itemAnalyticyStats。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2f8f2a449ddb730b31275ba2789fb14ea4f279b6
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970627"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="9a96d-103">按间隔获取项目活动统计</span><span class="sxs-lookup"><span data-stu-id="9a96d-103">Get item activity stats by interval</span></span>

<span data-ttu-id="9a96d-104">获取在指定时间间隔内发生在此资源上的活动的[itemActivityStats][]资源的集合。</span><span class="sxs-lookup"><span data-stu-id="9a96d-104">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="9a96d-105">**注意:\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9a96d-105">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="9a96d-106">分析聚合可能不适用于所有操作类型。</span><span class="sxs-lookup"><span data-stu-id="9a96d-106">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a96d-107">权限</span><span class="sxs-lookup"><span data-stu-id="9a96d-107">Permissions</span></span>

<span data-ttu-id="9a96d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a96d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a96d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a96d-110">Permission type</span></span>                        | <span data-ttu-id="9a96d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a96d-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="9a96d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a96d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a96d-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a96d-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="9a96d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a96d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a96d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a96d-115">Not supported.</span></span>
|<span data-ttu-id="9a96d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a96d-116">Application</span></span>                            | <span data-ttu-id="9a96d-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a96d-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="9a96d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a96d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="9a96d-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="9a96d-119">Function parameters</span></span>

| <span data-ttu-id="9a96d-120">参数</span><span class="sxs-lookup"><span data-stu-id="9a96d-120">Parameter</span></span>      | <span data-ttu-id="9a96d-121">类型</span><span class="sxs-lookup"><span data-stu-id="9a96d-121">Type</span></span>               | <span data-ttu-id="9a96d-122">说明</span><span class="sxs-lookup"><span data-stu-id="9a96d-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="9a96d-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9a96d-123">startDateTime</span></span>  | <span data-ttu-id="9a96d-124">字符串 (时间戳)</span><span class="sxs-lookup"><span data-stu-id="9a96d-124">string (timestamp)</span></span> | <span data-ttu-id="9a96d-125">聚合活动的开始时间。</span><span class="sxs-lookup"><span data-stu-id="9a96d-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="9a96d-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9a96d-126">endDateTime</span></span>    | <span data-ttu-id="9a96d-127">字符串 (时间戳)</span><span class="sxs-lookup"><span data-stu-id="9a96d-127">string (timestamp)</span></span> | <span data-ttu-id="9a96d-128">聚合活动的结束时间。</span><span class="sxs-lookup"><span data-stu-id="9a96d-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="9a96d-129">interval</span><span class="sxs-lookup"><span data-stu-id="9a96d-129">interval</span></span>       | <span data-ttu-id="9a96d-130">string</span><span class="sxs-lookup"><span data-stu-id="9a96d-130">string</span></span>             | <span data-ttu-id="9a96d-131">聚合间隔。</span><span class="sxs-lookup"><span data-stu-id="9a96d-131">The aggregation interval.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="9a96d-132">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9a96d-132">Optional query parameters</span></span>
<span data-ttu-id="9a96d-133">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9a96d-133">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a96d-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a96d-134">Request headers</span></span>

| <span data-ttu-id="9a96d-135">名称</span><span class="sxs-lookup"><span data-stu-id="9a96d-135">Name</span></span>      |<span data-ttu-id="9a96d-136">说明</span><span class="sxs-lookup"><span data-stu-id="9a96d-136">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a96d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a96d-137">Authorization</span></span>  | <span data-ttu-id="9a96d-138">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="9a96d-138">Bearer {code}.</span></span> <span data-ttu-id="9a96d-139">必需。</span><span class="sxs-lookup"><span data-stu-id="9a96d-139">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a96d-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a96d-140">Request body</span></span>

<span data-ttu-id="9a96d-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9a96d-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a96d-142">响应</span><span class="sxs-lookup"><span data-stu-id="9a96d-142">Response</span></span> 

<span data-ttu-id="9a96d-143">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[itemActivityStats][]对象集合。</span><span class="sxs-lookup"><span data-stu-id="9a96d-143">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="9a96d-144">示例</span><span class="sxs-lookup"><span data-stu-id="9a96d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a96d-145">请求</span><span class="sxs-lookup"><span data-stu-id="9a96d-145">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

### <a name="response"></a><span data-ttu-id="9a96d-146">响应</span><span class="sxs-lookup"><span data-stu-id="9a96d-146">Response</span></span>

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
[itemActivityStats]: ../resources/itemactivitystat.md

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
