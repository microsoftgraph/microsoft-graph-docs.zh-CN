---
title: 列出趋势
description: 计算的洞察力, 可返回围绕用户的项目趋势分析的列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 49f777e77663a4c055e186860f791459db57ca9c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323679"
---
# <a name="list-trending"></a><span data-ttu-id="f7fd6-103">列出趋势</span><span class="sxs-lookup"><span data-stu-id="f7fd6-103">List trending</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7fd6-104">计算的洞察力, 可返回围绕用户的项目趋势分析的列表。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-104">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7fd6-105">权限</span><span class="sxs-lookup"><span data-stu-id="f7fd6-105">Permissions</span></span>
<span data-ttu-id="f7fd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f7fd6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7fd6-108">Permission type</span></span>      | <span data-ttu-id="f7fd6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7fd6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7fd6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7fd6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7fd6-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7fd6-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7fd6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7fd6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7fd6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-113">Not supported.</span></span>    |
|<span data-ttu-id="f7fd6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7fd6-114">Application</span></span> | <span data-ttu-id="f7fd6-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7fd6-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7fd6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7fd6-116">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7fd6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f7fd6-117">Optional query parameters</span></span>
<span data-ttu-id="f7fd6-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f7fd6-119">您可以使用`$filter`查询参数筛选趋势项。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-119">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="f7fd6-120">例如, 基于类型:</span><span class="sxs-lookup"><span data-stu-id="f7fd6-120">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="f7fd6-121">或基于容器类型:</span><span class="sxs-lookup"><span data-stu-id="f7fd6-121">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="f7fd6-122">请参阅可在[resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="f7fd6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7fd6-123">Request headers</span></span>
| <span data-ttu-id="f7fd6-124">标头</span><span class="sxs-lookup"><span data-stu-id="f7fd6-124">Header</span></span>       |  <span data-ttu-id="f7fd6-125">值</span><span class="sxs-lookup"><span data-stu-id="f7fd6-125">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="f7fd6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7fd6-126">Authorization</span></span>  | <span data-ttu-id="f7fd6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f7fd6-129">接受</span><span class="sxs-lookup"><span data-stu-id="f7fd6-129">Accept</span></span>  | <span data-ttu-id="f7fd6-130">application/json</span><span class="sxs-lookup"><span data-stu-id="f7fd6-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7fd6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7fd6-131">Request body</span></span>
<span data-ttu-id="f7fd6-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7fd6-133">响应</span><span class="sxs-lookup"><span data-stu-id="f7fd6-133">Response</span></span>

<span data-ttu-id="f7fd6-134">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[趋势](../resources/insights-trending.md)项列表。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-134">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="f7fd6-135">每个项目都包含可视化属性, 用于显示您的体验中的项目。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-135">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="f7fd6-136">示例</span><span class="sxs-lookup"><span data-stu-id="f7fd6-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f7fd6-137">请求</span><span class="sxs-lookup"><span data-stu-id="f7fd6-137">Request</span></span>
<span data-ttu-id="f7fd6-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="f7fd6-139">响应</span><span class="sxs-lookup"><span data-stu-id="f7fd6-139">Response</span></span>
<span data-ttu-id="f7fd6-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-140">Here is an example of the response.</span></span> <span data-ttu-id="f7fd6-141">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f7fd6-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-142">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="f7fd6-143">请参阅页面底部的 "未截断的示例" 响应。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-143">See an example un-truncated response at the bottom of the page.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="f7fd6-144">扩展资源</span><span class="sxs-lookup"><span data-stu-id="f7fd6-144">Expanding resource</span></span>
<span data-ttu-id="f7fd6-145">可展开趋势洞察力引用的资源。</span><span class="sxs-lookup"><span data-stu-id="f7fd6-145">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
