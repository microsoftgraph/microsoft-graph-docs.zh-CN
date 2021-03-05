---
author: daspek
title: 获取 itemAnalytics
description: 获取有关此资源下发生视图的 itemAnalytics。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 25965acd48ca69b68f0715d9e075a5e71d5d1529
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471682"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="c5079-103">获取 itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="c5079-103">Get itemAnalytics</span></span>

<span data-ttu-id="c5079-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5079-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5079-105">获取有关此资源下发生视图的[itemAnalytics。][]</span><span class="sxs-lookup"><span data-stu-id="c5079-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="c5079-106">**itemAnalytics** 资源是获取 和 的活动统计信息的 `allTime` 便捷方式 `lastSevenDays` 。</span><span class="sxs-lookup"><span data-stu-id="c5079-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="c5079-107">对于自定义的时间间隔，请使用 [getActivitiesByInterval][] API。</span><span class="sxs-lookup"><span data-stu-id="c5079-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="c5079-108">**注意：\*\*\*\*itemAnalytics** 资源尚未在所有的国家部署 [中可用](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="c5079-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="c5079-111">权限</span><span class="sxs-lookup"><span data-stu-id="c5079-111">Permissions</span></span>

<span data-ttu-id="c5079-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5079-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5079-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5079-114">Permission type</span></span>                        | <span data-ttu-id="c5079-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5079-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c5079-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5079-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5079-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5079-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c5079-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5079-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5079-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5079-119">Not supported.</span></span>
|<span data-ttu-id="c5079-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5079-120">Application</span></span>                            | <span data-ttu-id="c5079-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5079-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c5079-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5079-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5079-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5079-123">Optional query parameters</span></span>
<span data-ttu-id="c5079-124">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c5079-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5079-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5079-125">Request headers</span></span>

| <span data-ttu-id="c5079-126">名称</span><span class="sxs-lookup"><span data-stu-id="c5079-126">Name</span></span>      |<span data-ttu-id="c5079-127">说明</span><span class="sxs-lookup"><span data-stu-id="c5079-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5079-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5079-128">Authorization</span></span>  | <span data-ttu-id="c5079-129">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="c5079-129">Bearer {code}.</span></span> <span data-ttu-id="c5079-130">必需。</span><span class="sxs-lookup"><span data-stu-id="c5079-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5079-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5079-131">Request body</span></span>

<span data-ttu-id="c5079-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5079-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5079-133">响应</span><span class="sxs-lookup"><span data-stu-id="c5079-133">Response</span></span> 

<span data-ttu-id="c5079-134">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [itemAnalytics][] 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c5079-134">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="c5079-135">示例</span><span class="sxs-lookup"><span data-stu-id="c5079-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5079-136">请求</span><span class="sxs-lookup"><span data-stu-id="c5079-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c5079-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5079-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="c5079-138">C#</span><span class="sxs-lookup"><span data-stu-id="c5079-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5079-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5079-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5079-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5079-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5079-141">Java</span><span class="sxs-lookup"><span data-stu-id="c5079-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5079-142">响应</span><span class="sxs-lookup"><span data-stu-id="c5079-142">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```http
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

