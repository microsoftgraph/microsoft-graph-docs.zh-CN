---
title: 列出趋势
description: 计算得出的见解，可返回用户常用的项目列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d5f0dbfe0b27a44f48d0be947e15ef20a980e935
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059612"
---
# <a name="list-trending"></a><span data-ttu-id="aed62-103">列出趋势</span><span class="sxs-lookup"><span data-stu-id="aed62-103">List trending</span></span>

<span data-ttu-id="aed62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aed62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aed62-105">计算的洞察力，包括围绕用户的文档趋势的列表。</span><span class="sxs-lookup"><span data-stu-id="aed62-105">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="aed62-106">权限</span><span class="sxs-lookup"><span data-stu-id="aed62-106">Permissions</span></span>
<span data-ttu-id="aed62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aed62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aed62-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aed62-109">Permission type</span></span>      | <span data-ttu-id="aed62-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aed62-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aed62-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aed62-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aed62-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aed62-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="aed62-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aed62-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aed62-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed62-114">Not supported.</span></span>    |
|<span data-ttu-id="aed62-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aed62-115">Application</span></span> | <span data-ttu-id="aed62-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aed62-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aed62-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aed62-117">HTTP request</span></span>
<span data-ttu-id="aed62-118">获取围绕登录用户或指定用户的文档趋势的列表：</span><span class="sxs-lookup"><span data-stu-id="aed62-118">Get a list of documents trending around the signed-in user or specified user:</span></span>

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="aed62-119">扩展 **趋势** 洞察力引用的资源：</span><span class="sxs-lookup"><span data-stu-id="aed62-119">Expand the resource referenced by a **trending** insight:</span></span>

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aed62-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aed62-120">Optional query parameters</span></span>
<span data-ttu-id="aed62-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aed62-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="aed62-122">您可以使用 `$filter` 查询参数筛选趋势项。</span><span class="sxs-lookup"><span data-stu-id="aed62-122">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="aed62-123">例如，基于 **类型**：</span><span class="sxs-lookup"><span data-stu-id="aed62-123">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="aed62-124">或基于 **containerType**：</span><span class="sxs-lookup"><span data-stu-id="aed62-124">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="aed62-125">请参阅可在 [resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="aed62-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="aed62-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="aed62-126">Request headers</span></span>
| <span data-ttu-id="aed62-127">标头</span><span class="sxs-lookup"><span data-stu-id="aed62-127">Header</span></span>       |  <span data-ttu-id="aed62-128">值</span><span class="sxs-lookup"><span data-stu-id="aed62-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="aed62-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="aed62-129">Authorization</span></span>  | <span data-ttu-id="aed62-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aed62-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="aed62-132">接受</span><span class="sxs-lookup"><span data-stu-id="aed62-132">Accept</span></span>  | <span data-ttu-id="aed62-133">application/json</span><span class="sxs-lookup"><span data-stu-id="aed62-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aed62-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="aed62-134">Request body</span></span>
<span data-ttu-id="aed62-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aed62-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aed62-136">响应</span><span class="sxs-lookup"><span data-stu-id="aed62-136">Response</span></span>

<span data-ttu-id="aed62-137">如果成功，此方法在 `200 OK` 响应正文中返回响应代码和 [趋势](../resources/insights-trending.md) 项列表。</span><span class="sxs-lookup"><span data-stu-id="aed62-137">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="aed62-138">每个项目都包含可视化属性，用于显示您的体验中的项目。</span><span class="sxs-lookup"><span data-stu-id="aed62-138">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="aed62-139">示例</span><span class="sxs-lookup"><span data-stu-id="aed62-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="aed62-140">请求</span><span class="sxs-lookup"><span data-stu-id="aed62-140">Request</span></span>
<span data-ttu-id="aed62-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aed62-141">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="aed62-142">响应</span><span class="sxs-lookup"><span data-stu-id="aed62-142">Response</span></span>
<span data-ttu-id="aed62-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aed62-143">Here is an example of the response.</span></span> <span data-ttu-id="aed62-144">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aed62-144">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="aed62-145">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aed62-145">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="aed62-146">请参阅页面底部的 "未截断的示例" 响应。</span><span class="sxs-lookup"><span data-stu-id="aed62-146">See an example un-truncated response at the bottom of the page.</span></span>
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



