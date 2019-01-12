---
title: 使用列表
description: 返回与用户使用的文件列表的计算的洞察。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 107e9429228bbedf131ae4ca4adde79e280cedb9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990631"
---
# <a name="list-used"></a><span data-ttu-id="a1e8c-103">使用列表</span><span class="sxs-lookup"><span data-stu-id="a1e8c-103">List used</span></span>

> <span data-ttu-id="a1e8c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1e8c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1e8c-106">返回与用户使用的文件列表的计算的洞察。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-106">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1e8c-107">权限</span><span class="sxs-lookup"><span data-stu-id="a1e8c-107">Permissions</span></span>
<span data-ttu-id="a1e8c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1e8c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1e8c-110">Permission type</span></span>      | <span data-ttu-id="a1e8c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1e8c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1e8c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1e8c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a1e8c-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1e8c-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a1e8c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1e8c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1e8c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-115">Not supported.</span></span>    |
|<span data-ttu-id="a1e8c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1e8c-116">Application</span></span> | <span data-ttu-id="a1e8c-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1e8c-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1e8c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1e8c-118">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="a1e8c-119">请求其他用户使用的文档返回结果按 lastModifiedDateTime' 和 'lastAccessedDateTime 设置为 lastModifiedDateTime。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-119">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1e8c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a1e8c-120">Optional query parameters</span></span>
<span data-ttu-id="a1e8c-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a1e8c-122">您可以使用`$filter`查询参数使用筛选器的项目。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-122">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="a1e8c-123">例如，基于类型：</span><span class="sxs-lookup"><span data-stu-id="a1e8c-123">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="a1e8c-124">还是基于容器类型：</span><span class="sxs-lookup"><span data-stu-id="a1e8c-124">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="a1e8c-125">请参阅可用的容器类型和[resourceVisualization](../resources/insights-resourcevisualization.md)中可以通过筛选的类型。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-125">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="a1e8c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1e8c-126">Request headers</span></span>
| <span data-ttu-id="a1e8c-127">标头</span><span class="sxs-lookup"><span data-stu-id="a1e8c-127">Header</span></span>       |  <span data-ttu-id="a1e8c-128">值</span><span class="sxs-lookup"><span data-stu-id="a1e8c-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="a1e8c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1e8c-129">Authorization</span></span>  | <span data-ttu-id="a1e8c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a1e8c-132">Accept</span><span class="sxs-lookup"><span data-stu-id="a1e8c-132">Accept</span></span>  | <span data-ttu-id="a1e8c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="a1e8c-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1e8c-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1e8c-134">Request body</span></span>
<span data-ttu-id="a1e8c-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1e8c-136">响应</span><span class="sxs-lookup"><span data-stu-id="a1e8c-136">Response</span></span>

<span data-ttu-id="a1e8c-137">如果成功，此方法返回`200 OK`响应代码以及响应正文中[使用](../resources/insights-used.md)项目的列表。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-137">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1e8c-138">示例</span><span class="sxs-lookup"><span data-stu-id="a1e8c-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a1e8c-139">请求</span><span class="sxs-lookup"><span data-stu-id="a1e8c-139">Request</span></span>

<span data-ttu-id="a1e8c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="a1e8c-141">响应</span><span class="sxs-lookup"><span data-stu-id="a1e8c-141">Response</span></span>

<span data-ttu-id="a1e8c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
            }
        }
    ]
}
```

### <a name="expanding-resource"></a><span data-ttu-id="a1e8c-145">展开资源</span><span class="sxs-lookup"><span data-stu-id="a1e8c-145">Expanding resource</span></span>
<span data-ttu-id="a1e8c-146">可以扩展使用洞察引用的资源。</span><span class="sxs-lookup"><span data-stu-id="a1e8c-146">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
