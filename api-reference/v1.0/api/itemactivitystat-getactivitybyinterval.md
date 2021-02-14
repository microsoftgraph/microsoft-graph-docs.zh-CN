---
author: daspek
title: 按间隔获取项目活动统计信息
description: 获取指定时间间隔内在此资源上发生活动的 itemAnalyticyStats。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a0ce73166603831c5cf870a6b969f1844c81ffb4
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238580"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="bd2b9-103">按间隔获取项目活动统计信息</span><span class="sxs-lookup"><span data-stu-id="bd2b9-103">Get item activity stats by interval</span></span>

<span data-ttu-id="bd2b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd2b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bd2b9-105">获取指定时间间隔内在此资源上发生活动的 [itemActivityStats][] 资源集合。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-105">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="bd2b9-106">**注意：\*\*\*\*itemAnalytics** 资源尚未在所有的国家部署 [中可用](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span> 

<span data-ttu-id="bd2b9-107">分析聚合可能并非可用于所有操作类型。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-107">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd2b9-108">权限</span><span class="sxs-lookup"><span data-stu-id="bd2b9-108">Permissions</span></span>

<span data-ttu-id="bd2b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd2b9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd2b9-111">Permission type</span></span>                        | <span data-ttu-id="bd2b9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd2b9-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="bd2b9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd2b9-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd2b9-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd2b9-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="bd2b9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd2b9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd2b9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-116">Not supported.</span></span>
|<span data-ttu-id="bd2b9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd2b9-117">Application</span></span>                            | <span data-ttu-id="bd2b9-118">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd2b9-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="bd2b9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd2b9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016-01-01',endDateTime='2017-05-20',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="bd2b9-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="bd2b9-120">Function parameters</span></span>

| <span data-ttu-id="bd2b9-121">参数</span><span class="sxs-lookup"><span data-stu-id="bd2b9-121">Parameter</span></span>      | <span data-ttu-id="bd2b9-122">类型</span><span class="sxs-lookup"><span data-stu-id="bd2b9-122">Type</span></span>               | <span data-ttu-id="bd2b9-123">说明</span><span class="sxs-lookup"><span data-stu-id="bd2b9-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="bd2b9-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bd2b9-124">startDateTime</span></span>  | <span data-ttu-id="bd2b9-125">字符串 (时间戳) </span><span class="sxs-lookup"><span data-stu-id="bd2b9-125">string (timestamp)</span></span> | <span data-ttu-id="bd2b9-126">聚合活动的开始时间。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="bd2b9-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bd2b9-127">endDateTime</span></span>    | <span data-ttu-id="bd2b9-128">字符串 (时间戳) </span><span class="sxs-lookup"><span data-stu-id="bd2b9-128">string (timestamp)</span></span> | <span data-ttu-id="bd2b9-129">聚合活动的结束时间。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="bd2b9-130">interval</span><span class="sxs-lookup"><span data-stu-id="bd2b9-130">interval</span></span>       | <span data-ttu-id="bd2b9-131">string</span><span class="sxs-lookup"><span data-stu-id="bd2b9-131">string</span></span>             | <span data-ttu-id="bd2b9-132">聚合间隔。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-132">The aggregation interval.</span></span>

><span data-ttu-id="bd2b9-133">**注意：** 此 API 仅支持每日计数的 90 天时间范围。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-133">**Note:** This API only supports a time range of 90 days for daily counts.</span></span> <span data-ttu-id="bd2b9-134">和参数的值 `startDateTime` `endDateTime` 必须表示小于 90 天的时区。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-134">The value of the `startDateTime` and `endDateTime` parameters must represent a time range of less than 90 days.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="bd2b9-135">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bd2b9-135">Optional query parameters</span></span>
<span data-ttu-id="bd2b9-136">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-136">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd2b9-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd2b9-137">Request headers</span></span>

| <span data-ttu-id="bd2b9-138">名称</span><span class="sxs-lookup"><span data-stu-id="bd2b9-138">Name</span></span>      |<span data-ttu-id="bd2b9-139">说明</span><span class="sxs-lookup"><span data-stu-id="bd2b9-139">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd2b9-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd2b9-140">Authorization</span></span>  | <span data-ttu-id="bd2b9-141">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-141">Bearer {code}.</span></span> <span data-ttu-id="bd2b9-142">必需。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-142">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd2b9-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd2b9-143">Request body</span></span>

<span data-ttu-id="bd2b9-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd2b9-145">响应</span><span class="sxs-lookup"><span data-stu-id="bd2b9-145">Response</span></span> 

<span data-ttu-id="bd2b9-146">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [itemActivityStats][] 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bd2b9-146">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="bd2b9-147">示例</span><span class="sxs-lookup"><span data-stu-id="bd2b9-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd2b9-148">请求</span><span class="sxs-lookup"><span data-stu-id="bd2b9-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bd2b9-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd2b9-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="bd2b9-150">C#</span><span class="sxs-lookup"><span data-stu-id="bd2b9-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd2b9-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd2b9-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd2b9-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd2b9-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd2b9-153">Java</span><span class="sxs-lookup"><span data-stu-id="bd2b9-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activities-by-interval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd2b9-154">响应</span><span class="sxs-lookup"><span data-stu-id="bd2b9-154">Response</span></span>

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

