---
title: 列出趋势
description: 计算得出的见解，可返回用户常用的项目列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: e97e5f9a72084b7748551d60e795e43e80f353ed
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844350"
---
# <a name="list-trending"></a><span data-ttu-id="4e237-103">列出趋势</span><span class="sxs-lookup"><span data-stu-id="4e237-103">List trending</span></span>

<span data-ttu-id="4e237-104">计算的洞察力，包括围绕用户的文档趋势的列表。</span><span class="sxs-lookup"><span data-stu-id="4e237-104">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e237-105">权限</span><span class="sxs-lookup"><span data-stu-id="4e237-105">Permissions</span></span>
<span data-ttu-id="4e237-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e237-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4e237-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e237-108">Permission type</span></span>      | <span data-ttu-id="4e237-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e237-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e237-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e237-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4e237-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e237-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e237-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e237-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e237-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e237-113">Not supported.</span></span>    |
|<span data-ttu-id="4e237-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e237-114">Application</span></span> | <span data-ttu-id="4e237-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e237-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e237-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e237-116">HTTP request</span></span>
<span data-ttu-id="4e237-117">获取围绕登录用户或指定用户的文档趋势的列表：</span><span class="sxs-lookup"><span data-stu-id="4e237-117">Get a list of documents trending around the signed-in user or specified user:</span></span>

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="4e237-118">扩展**趋势**洞察力引用的资源：</span><span class="sxs-lookup"><span data-stu-id="4e237-118">Expand the resource referenced by a **trending** insight:</span></span>

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e237-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4e237-119">Optional query parameters</span></span>
<span data-ttu-id="4e237-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4e237-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4e237-121">您可以使用`$filter`查询参数筛选趋势项。</span><span class="sxs-lookup"><span data-stu-id="4e237-121">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="4e237-122">例如，基于**类型**：</span><span class="sxs-lookup"><span data-stu-id="4e237-122">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="4e237-123">或基于**containerType**：</span><span class="sxs-lookup"><span data-stu-id="4e237-123">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="4e237-124">请参阅可在[resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="4e237-124">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="4e237-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e237-125">Request headers</span></span>
| <span data-ttu-id="4e237-126">标头</span><span class="sxs-lookup"><span data-stu-id="4e237-126">Header</span></span>       |  <span data-ttu-id="4e237-127">值</span><span class="sxs-lookup"><span data-stu-id="4e237-127">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="4e237-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e237-128">Authorization</span></span>  | <span data-ttu-id="4e237-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e237-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4e237-131">接受</span><span class="sxs-lookup"><span data-stu-id="4e237-131">Accept</span></span>  | <span data-ttu-id="4e237-132">application/json</span><span class="sxs-lookup"><span data-stu-id="4e237-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e237-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e237-133">Request body</span></span>
<span data-ttu-id="4e237-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e237-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e237-135">响应</span><span class="sxs-lookup"><span data-stu-id="4e237-135">Response</span></span>

<span data-ttu-id="4e237-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和[趋势](../resources/insights-trending.md)项列表。</span><span class="sxs-lookup"><span data-stu-id="4e237-136">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="4e237-137">每个项目都包含可视化属性，用于显示您的体验中的项目。</span><span class="sxs-lookup"><span data-stu-id="4e237-137">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="4e237-138">示例</span><span class="sxs-lookup"><span data-stu-id="4e237-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4e237-139">请求</span><span class="sxs-lookup"><span data-stu-id="4e237-139">Request</span></span>
<span data-ttu-id="4e237-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e237-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="4e237-141">响应</span><span class="sxs-lookup"><span data-stu-id="4e237-141">Response</span></span>
<span data-ttu-id="4e237-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4e237-142">Here is an example of the response.</span></span> <span data-ttu-id="4e237-143">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4e237-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4e237-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4e237-144">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="4e237-145">请参阅页面底部的 "未截断的示例" 响应。</span><span class="sxs-lookup"><span data-stu-id="4e237-145">See an example un-truncated response at the bottom of the page.</span></span>
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


