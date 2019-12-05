---
title: 使用的列表
description: 计算得出的见解，可返回用户使用的文件列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 8a9a1114b5e247807b952d15901b5def124a245a
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844348"
---
# <a name="list-used"></a><span data-ttu-id="d668e-103">使用的列表</span><span class="sxs-lookup"><span data-stu-id="d668e-103">List used</span></span>

<span data-ttu-id="d668e-104">计算的洞察力，包括用户修改的文档列表。</span><span class="sxs-lookup"><span data-stu-id="d668e-104">Calculated insight that includes a list of documents the user has modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="d668e-105">权限</span><span class="sxs-lookup"><span data-stu-id="d668e-105">Permissions</span></span>
<span data-ttu-id="d668e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d668e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d668e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d668e-108">Permission type</span></span>      | <span data-ttu-id="d668e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d668e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d668e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d668e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d668e-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d668e-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d668e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d668e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d668e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d668e-113">Not supported.</span></span>    |
|<span data-ttu-id="d668e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d668e-114">Application</span></span> | <span data-ttu-id="d668e-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d668e-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d668e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d668e-116">HTTP request</span></span>
<span data-ttu-id="d668e-117">获取已登录用户已修改的文档列表：</span><span class="sxs-lookup"><span data-stu-id="d668e-117">Get a list of documents that the signed-in user has modified:</span></span>

```http
GET /me/insights/used
```

<span data-ttu-id="d668e-118">获取指定用户已修改的文档列表。</span><span class="sxs-lookup"><span data-stu-id="d668e-118">Get a list of documents that the specified user has modified.</span></span>

><span data-ttu-id="d668e-119">**注意**：请求其他用户的已**使用**文档返回按**lastModifiedDateTime**排序的结果。</span><span class="sxs-lookup"><span data-stu-id="d668e-119">**Note**: Requesting another user's **used** documents returns results sorted by **lastModifiedDateTime**.</span></span> <span data-ttu-id="d668e-120">然后，将**lastAccessedDateTime**设置为**lastModifiedDateTime**。</span><span class="sxs-lookup"><span data-stu-id="d668e-120">**lastAccessedDateTime** is then set to **lastModifiedDateTime**.</span></span>
```http
GET /users/{id | userPrincipalName}/insights/used
```

<span data-ttu-id="d668e-121">扩展**使用**的洞察力引用的资源：</span><span class="sxs-lookup"><span data-stu-id="d668e-121">Expand the resource referenced by a **used** insight:</span></span>

```http
GET /me/insights/used/{id}/resource
GET /users/{id | userPrincipalName}/insights/used/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d668e-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d668e-122">Optional query parameters</span></span>
<span data-ttu-id="d668e-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d668e-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d668e-124">您可以使用`$filter`查询参数筛选已使用的项目。</span><span class="sxs-lookup"><span data-stu-id="d668e-124">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="d668e-125">例如，基于**类型**：</span><span class="sxs-lookup"><span data-stu-id="d668e-125">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="d668e-126">或基于**containerType**：</span><span class="sxs-lookup"><span data-stu-id="d668e-126">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="d668e-127">请参阅可在[resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="d668e-127">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="d668e-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="d668e-128">Request headers</span></span>
| <span data-ttu-id="d668e-129">标头</span><span class="sxs-lookup"><span data-stu-id="d668e-129">Header</span></span>       |  <span data-ttu-id="d668e-130">值</span><span class="sxs-lookup"><span data-stu-id="d668e-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="d668e-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d668e-131">Authorization</span></span>  | <span data-ttu-id="d668e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d668e-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d668e-134">接受</span><span class="sxs-lookup"><span data-stu-id="d668e-134">Accept</span></span>  | <span data-ttu-id="d668e-135">application/json</span><span class="sxs-lookup"><span data-stu-id="d668e-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d668e-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="d668e-136">Request body</span></span>
<span data-ttu-id="d668e-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d668e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d668e-138">响应</span><span class="sxs-lookup"><span data-stu-id="d668e-138">Response</span></span>

<span data-ttu-id="d668e-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和已[使用](../resources/insights-used.md)项的列表。</span><span class="sxs-lookup"><span data-stu-id="d668e-139">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d668e-140">示例</span><span class="sxs-lookup"><span data-stu-id="d668e-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d668e-141">请求</span><span class="sxs-lookup"><span data-stu-id="d668e-141">Request</span></span>

<span data-ttu-id="d668e-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d668e-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="d668e-143">响应</span><span class="sxs-lookup"><span data-stu-id="d668e-143">Response</span></span>

<span data-ttu-id="d668e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d668e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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


