---
author: daspek
ms.author: dspektor
title: 获取 itemAnalytics
description: 获取有关在此资源下发生的视图的 itemAnalytics。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 311d7eea81ba3001af6cb94e2a3f837824a67fde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038471"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="de638-103">获取 itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="de638-103">Get itemAnalytics</span></span>

<span data-ttu-id="de638-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de638-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de638-105">获取有关在此资源下发生的视图的 [itemAnalytics][] 。</span><span class="sxs-lookup"><span data-stu-id="de638-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="de638-106">**ItemAnalytics**资源是获取和的活动统计信息的便捷方式 `allTime` `lastSevenDays` 。</span><span class="sxs-lookup"><span data-stu-id="de638-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="de638-107">对于自定义时间范围或时间间隔，请使用 [getActivitiesByInterval][] API。</span><span class="sxs-lookup"><span data-stu-id="de638-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="de638-108">**注意：\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="de638-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="de638-111">权限</span><span class="sxs-lookup"><span data-stu-id="de638-111">Permissions</span></span>

<span data-ttu-id="de638-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de638-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de638-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="de638-114">Permission type</span></span>                        | <span data-ttu-id="de638-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de638-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="de638-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de638-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="de638-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de638-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="de638-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de638-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de638-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="de638-119">Not supported.</span></span>
|<span data-ttu-id="de638-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="de638-120">Application</span></span>                            | <span data-ttu-id="de638-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de638-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="de638-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de638-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="de638-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="de638-123">Optional query parameters</span></span>
<span data-ttu-id="de638-124">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="de638-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de638-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="de638-125">Request headers</span></span>

| <span data-ttu-id="de638-126">名称</span><span class="sxs-lookup"><span data-stu-id="de638-126">Name</span></span>      |<span data-ttu-id="de638-127">说明</span><span class="sxs-lookup"><span data-stu-id="de638-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="de638-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="de638-128">Authorization</span></span>  | <span data-ttu-id="de638-129">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="de638-129">Bearer {code}.</span></span> <span data-ttu-id="de638-130">必需。</span><span class="sxs-lookup"><span data-stu-id="de638-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de638-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="de638-131">Request body</span></span>

<span data-ttu-id="de638-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="de638-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de638-133">响应</span><span class="sxs-lookup"><span data-stu-id="de638-133">Response</span></span> 

<span data-ttu-id="de638-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [itemAnalytics][] 对象集合。</span><span class="sxs-lookup"><span data-stu-id="de638-134">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="de638-135">示例</span><span class="sxs-lookup"><span data-stu-id="de638-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="de638-136">请求</span><span class="sxs-lookup"><span data-stu-id="de638-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="de638-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="de638-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="de638-138">C#</span><span class="sxs-lookup"><span data-stu-id="de638-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de638-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de638-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de638-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de638-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de638-141">Java</span><span class="sxs-lookup"><span data-stu-id="de638-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="de638-142">响应</span><span class="sxs-lookup"><span data-stu-id="de638-142">Response</span></span>

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

