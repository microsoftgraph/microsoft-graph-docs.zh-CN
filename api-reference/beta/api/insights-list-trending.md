---
title: 列表趋势分析
description: 返回用户周围趋势分析的项的列表的计算的洞察。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 86b9daf96529d50d8767f234c3b1a6d9526eaac4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854787"
---
# <a name="list-trending"></a><span data-ttu-id="014ad-103">列表趋势分析</span><span class="sxs-lookup"><span data-stu-id="014ad-103">List trending</span></span>

> <span data-ttu-id="014ad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="014ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="014ad-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="014ad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="014ad-106">返回用户周围趋势分析的项的列表的计算的洞察。</span><span class="sxs-lookup"><span data-stu-id="014ad-106">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="014ad-107">权限</span><span class="sxs-lookup"><span data-stu-id="014ad-107">Permissions</span></span>
<span data-ttu-id="014ad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="014ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="014ad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="014ad-110">Permission type</span></span>      | <span data-ttu-id="014ad-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="014ad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="014ad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="014ad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="014ad-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="014ad-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="014ad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="014ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="014ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="014ad-115">Not supported.</span></span>    |
|<span data-ttu-id="014ad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="014ad-116">Application</span></span> | <span data-ttu-id="014ad-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="014ad-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="014ad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="014ad-118">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="014ad-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="014ad-119">Optional query parameters</span></span>
<span data-ttu-id="014ad-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="014ad-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="014ad-121">您可以使用`$filter`查询参数趋势项进行筛选。</span><span class="sxs-lookup"><span data-stu-id="014ad-121">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="014ad-122">例如，基于类型：</span><span class="sxs-lookup"><span data-stu-id="014ad-122">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="014ad-123">还是基于容器类型：</span><span class="sxs-lookup"><span data-stu-id="014ad-123">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="014ad-124">请参阅可用的容器类型和[resourceVisualization](../resources/insights-resourcevisualization.md)中可以通过筛选的类型。</span><span class="sxs-lookup"><span data-stu-id="014ad-124">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="014ad-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="014ad-125">Request headers</span></span>
| <span data-ttu-id="014ad-126">标头</span><span class="sxs-lookup"><span data-stu-id="014ad-126">Header</span></span>       |  <span data-ttu-id="014ad-127">值</span><span class="sxs-lookup"><span data-stu-id="014ad-127">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="014ad-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="014ad-128">Authorization</span></span>  | <span data-ttu-id="014ad-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="014ad-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="014ad-131">Accept</span><span class="sxs-lookup"><span data-stu-id="014ad-131">Accept</span></span>  | <span data-ttu-id="014ad-132">application/json</span><span class="sxs-lookup"><span data-stu-id="014ad-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="014ad-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="014ad-133">Request body</span></span>
<span data-ttu-id="014ad-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="014ad-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="014ad-135">响应</span><span class="sxs-lookup"><span data-stu-id="014ad-135">Response</span></span>

<span data-ttu-id="014ad-136">如果成功，此方法返回`200 OK`响应代码以及响应正文中的[趋势分析](../resources/insights-trending.md)项目的列表。</span><span class="sxs-lookup"><span data-stu-id="014ad-136">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="014ad-137">每个项目包含在您的体验中显示项目的可视化效果属性。</span><span class="sxs-lookup"><span data-stu-id="014ad-137">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="014ad-138">示例</span><span class="sxs-lookup"><span data-stu-id="014ad-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="014ad-139">请求</span><span class="sxs-lookup"><span data-stu-id="014ad-139">Request</span></span>
<span data-ttu-id="014ad-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="014ad-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="014ad-141">响应</span><span class="sxs-lookup"><span data-stu-id="014ad-141">Response</span></span>
<span data-ttu-id="014ad-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="014ad-142">Here is an example of the response.</span></span> <span data-ttu-id="014ad-143">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="014ad-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="014ad-144">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="014ad-144">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="014ad-145">请参阅在页面底部示例未截断的响应。</span><span class="sxs-lookup"><span data-stu-id="014ad-145">See an example un-truncated response at the bottom of the page.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```

### <a name="expanding-resource"></a><span data-ttu-id="014ad-146">展开资源</span><span class="sxs-lookup"><span data-stu-id="014ad-146">Expanding resource</span></span>
<span data-ttu-id="014ad-147">可以扩展趋势洞察引用的资源。</span><span class="sxs-lookup"><span data-stu-id="014ad-147">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
