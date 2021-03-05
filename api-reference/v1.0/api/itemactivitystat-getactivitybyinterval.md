---
author: daspek
title: 按间隔获取项目活动统计信息
description: 获取指定时间间隔内在此资源上发生活动的 itemAnalyticyStats。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b339458fb65f457c44113957ef541828a1940724
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471690"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="98f50-103">按间隔获取项目活动统计信息</span><span class="sxs-lookup"><span data-stu-id="98f50-103">Get item activity stats by interval</span></span>

<span data-ttu-id="98f50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98f50-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="98f50-105">获取指定时间间隔内在此资源上发生活动的 [itemActivityStats][] 资源集合。</span><span class="sxs-lookup"><span data-stu-id="98f50-105">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="98f50-106">**注意：\*\*\*\*itemAnalytics** 资源尚未在所有的国家部署 [中可用](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="98f50-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span> 

<span data-ttu-id="98f50-107">分析聚合可能并非可用于所有操作类型。</span><span class="sxs-lookup"><span data-stu-id="98f50-107">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="98f50-108">权限</span><span class="sxs-lookup"><span data-stu-id="98f50-108">Permissions</span></span>

<span data-ttu-id="98f50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98f50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98f50-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="98f50-111">Permission type</span></span>                        | <span data-ttu-id="98f50-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98f50-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="98f50-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98f50-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="98f50-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98f50-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="98f50-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98f50-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98f50-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="98f50-116">Not supported.</span></span>
|<span data-ttu-id="98f50-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="98f50-117">Application</span></span>                            | <span data-ttu-id="98f50-118">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98f50-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="98f50-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98f50-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016-01-01',endDateTime='2017-05-20',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="98f50-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="98f50-120">Function parameters</span></span>

| <span data-ttu-id="98f50-121">参数</span><span class="sxs-lookup"><span data-stu-id="98f50-121">Parameter</span></span>      | <span data-ttu-id="98f50-122">类型</span><span class="sxs-lookup"><span data-stu-id="98f50-122">Type</span></span>               | <span data-ttu-id="98f50-123">说明</span><span class="sxs-lookup"><span data-stu-id="98f50-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="98f50-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="98f50-124">startDateTime</span></span>  | <span data-ttu-id="98f50-125">字符串 (时间戳) </span><span class="sxs-lookup"><span data-stu-id="98f50-125">string (timestamp)</span></span> | <span data-ttu-id="98f50-126">聚合活动的开始时间。</span><span class="sxs-lookup"><span data-stu-id="98f50-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="98f50-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="98f50-127">endDateTime</span></span>    | <span data-ttu-id="98f50-128">字符串 (时间戳) </span><span class="sxs-lookup"><span data-stu-id="98f50-128">string (timestamp)</span></span> | <span data-ttu-id="98f50-129">聚合活动的结束时间。</span><span class="sxs-lookup"><span data-stu-id="98f50-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="98f50-130">interval</span><span class="sxs-lookup"><span data-stu-id="98f50-130">interval</span></span>       | <span data-ttu-id="98f50-131">string</span><span class="sxs-lookup"><span data-stu-id="98f50-131">string</span></span>             | <span data-ttu-id="98f50-132">聚合间隔。</span><span class="sxs-lookup"><span data-stu-id="98f50-132">The aggregation interval.</span></span>

><span data-ttu-id="98f50-133">**注意：** 此 API 仅支持每日计数的 90 天时间范围。</span><span class="sxs-lookup"><span data-stu-id="98f50-133">**Note:** This API only supports a time range of 90 days for daily counts.</span></span> <span data-ttu-id="98f50-134">和参数的值 `startDateTime` `endDateTime` 必须表示小于 90 天的时区。</span><span class="sxs-lookup"><span data-stu-id="98f50-134">The value of the `startDateTime` and `endDateTime` parameters must represent a time range of less than 90 days.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="98f50-135">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="98f50-135">Optional query parameters</span></span>
<span data-ttu-id="98f50-136">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="98f50-136">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98f50-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="98f50-137">Request headers</span></span>

| <span data-ttu-id="98f50-138">名称</span><span class="sxs-lookup"><span data-stu-id="98f50-138">Name</span></span>      |<span data-ttu-id="98f50-139">说明</span><span class="sxs-lookup"><span data-stu-id="98f50-139">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98f50-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="98f50-140">Authorization</span></span>  | <span data-ttu-id="98f50-141">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="98f50-141">Bearer {code}.</span></span> <span data-ttu-id="98f50-142">必需。</span><span class="sxs-lookup"><span data-stu-id="98f50-142">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98f50-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="98f50-143">Request body</span></span>

<span data-ttu-id="98f50-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98f50-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98f50-145">响应</span><span class="sxs-lookup"><span data-stu-id="98f50-145">Response</span></span> 

<span data-ttu-id="98f50-146">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [itemActivityStats][] 对象集合。</span><span class="sxs-lookup"><span data-stu-id="98f50-146">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="98f50-147">示例</span><span class="sxs-lookup"><span data-stu-id="98f50-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="98f50-148">请求</span><span class="sxs-lookup"><span data-stu-id="98f50-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="98f50-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="98f50-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="98f50-150">C#</span><span class="sxs-lookup"><span data-stu-id="98f50-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98f50-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98f50-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98f50-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98f50-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98f50-153">Java</span><span class="sxs-lookup"><span data-stu-id="98f50-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activities-by-interval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="98f50-154">响应</span><span class="sxs-lookup"><span data-stu-id="98f50-154">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```http
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

