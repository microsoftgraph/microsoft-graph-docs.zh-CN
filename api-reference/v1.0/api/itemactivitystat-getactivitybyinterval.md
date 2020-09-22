---
author: daspek
ms.author: dspektor
title: 按间隔获取项目活动统计
description: 获取在指定时间间隔内发生在此资源上的活动的 itemAnalyticyStats。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a26892aac83aa28b7a4769f2ad678643a3c417ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087220"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="f761d-103">按间隔获取项目活动统计</span><span class="sxs-lookup"><span data-stu-id="f761d-103">Get item activity stats by interval</span></span>

<span data-ttu-id="f761d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f761d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f761d-105">获取在指定时间间隔内发生在此资源上的活动的 [itemActivityStats][] 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="f761d-105">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="f761d-106">**注意：\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="f761d-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span> 

<span data-ttu-id="f761d-107">分析聚合可能不适用于所有操作类型。</span><span class="sxs-lookup"><span data-stu-id="f761d-107">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="f761d-108">权限</span><span class="sxs-lookup"><span data-stu-id="f761d-108">Permissions</span></span>

<span data-ttu-id="f761d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f761d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f761d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f761d-111">Permission type</span></span>                        | <span data-ttu-id="f761d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f761d-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="f761d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f761d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f761d-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f761d-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="f761d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f761d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f761d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f761d-116">Not supported.</span></span>
|<span data-ttu-id="f761d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f761d-117">Application</span></span>                            | <span data-ttu-id="f761d-118">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f761d-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f761d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f761d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016-01-01',endDateTime='2017-05-20',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="f761d-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="f761d-120">Function parameters</span></span>

| <span data-ttu-id="f761d-121">参数</span><span class="sxs-lookup"><span data-stu-id="f761d-121">Parameter</span></span>      | <span data-ttu-id="f761d-122">类型</span><span class="sxs-lookup"><span data-stu-id="f761d-122">Type</span></span>               | <span data-ttu-id="f761d-123">说明</span><span class="sxs-lookup"><span data-stu-id="f761d-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="f761d-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f761d-124">startDateTime</span></span>  | <span data-ttu-id="f761d-125"> (时间戳) 的字符串</span><span class="sxs-lookup"><span data-stu-id="f761d-125">string (timestamp)</span></span> | <span data-ttu-id="f761d-126">聚合活动的开始时间。</span><span class="sxs-lookup"><span data-stu-id="f761d-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="f761d-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f761d-127">endDateTime</span></span>    | <span data-ttu-id="f761d-128"> (时间戳) 的字符串</span><span class="sxs-lookup"><span data-stu-id="f761d-128">string (timestamp)</span></span> | <span data-ttu-id="f761d-129">聚合活动的结束时间。</span><span class="sxs-lookup"><span data-stu-id="f761d-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="f761d-130">interval</span><span class="sxs-lookup"><span data-stu-id="f761d-130">interval</span></span>       | <span data-ttu-id="f761d-131">string</span><span class="sxs-lookup"><span data-stu-id="f761d-131">string</span></span>             | <span data-ttu-id="f761d-132">聚合间隔。</span><span class="sxs-lookup"><span data-stu-id="f761d-132">The aggregation interval.</span></span>

><span data-ttu-id="f761d-133">**注意：** 此 API 仅支持每日计数的90天的时间范围。</span><span class="sxs-lookup"><span data-stu-id="f761d-133">**Note:** This API only supports a time range of 90 days for daily counts.</span></span> <span data-ttu-id="f761d-134">和参数的值 `startDateTime` `endDateTime` 必须代表少于90天的时间范围。</span><span class="sxs-lookup"><span data-stu-id="f761d-134">The value of the `startDateTime` and `endDateTime` parameters must represent a time range of less than 90 days.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="f761d-135">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f761d-135">Optional query parameters</span></span>
<span data-ttu-id="f761d-136">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f761d-136">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f761d-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="f761d-137">Request headers</span></span>

| <span data-ttu-id="f761d-138">名称</span><span class="sxs-lookup"><span data-stu-id="f761d-138">Name</span></span>      |<span data-ttu-id="f761d-139">说明</span><span class="sxs-lookup"><span data-stu-id="f761d-139">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f761d-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="f761d-140">Authorization</span></span>  | <span data-ttu-id="f761d-141">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="f761d-141">Bearer {code}.</span></span> <span data-ttu-id="f761d-142">必需。</span><span class="sxs-lookup"><span data-stu-id="f761d-142">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f761d-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="f761d-143">Request body</span></span>

<span data-ttu-id="f761d-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f761d-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f761d-145">响应</span><span class="sxs-lookup"><span data-stu-id="f761d-145">Response</span></span> 

<span data-ttu-id="f761d-146">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [itemActivityStats][] 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f761d-146">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="f761d-147">示例</span><span class="sxs-lookup"><span data-stu-id="f761d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f761d-148">请求</span><span class="sxs-lookup"><span data-stu-id="f761d-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f761d-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="f761d-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="f761d-150">C#</span><span class="sxs-lookup"><span data-stu-id="f761d-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f761d-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f761d-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f761d-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f761d-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f761d-153">Java</span><span class="sxs-lookup"><span data-stu-id="f761d-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activities-by-interval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f761d-154">响应</span><span class="sxs-lookup"><span data-stu-id="f761d-154">Response</span></span>

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

