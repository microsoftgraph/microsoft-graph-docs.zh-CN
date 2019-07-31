---
title: 使用的列表
description: 计算出的洞察力, 可返回用户使用的文件列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 31115a845c3b5af80aaba700e55e0ede05d922b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953071"
---
# <a name="list-used"></a><span data-ttu-id="02262-103">使用的列表</span><span class="sxs-lookup"><span data-stu-id="02262-103">List used</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02262-104">计算出的洞察力, 可返回用户使用的文件列表。</span><span class="sxs-lookup"><span data-stu-id="02262-104">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="02262-105">权限</span><span class="sxs-lookup"><span data-stu-id="02262-105">Permissions</span></span>
<span data-ttu-id="02262-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02262-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02262-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="02262-108">Permission type</span></span>      | <span data-ttu-id="02262-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02262-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02262-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02262-110">Delegated (work or school account)</span></span> | <span data-ttu-id="02262-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02262-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="02262-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02262-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02262-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="02262-113">Not supported.</span></span>    |
|<span data-ttu-id="02262-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="02262-114">Application</span></span> | <span data-ttu-id="02262-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02262-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02262-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02262-116">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="02262-117">请求其他用户的已用文档返回按 "lastModifiedDateTime" 和 "lastAccessedDateTime" 排序的结果设置为 "lastModifiedDateTime"。</span><span class="sxs-lookup"><span data-stu-id="02262-117">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/{id | userPrincipalName}/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02262-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="02262-118">Optional query parameters</span></span>
<span data-ttu-id="02262-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="02262-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="02262-120">您可以使用`$filter`查询参数筛选已使用的项目。</span><span class="sxs-lookup"><span data-stu-id="02262-120">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="02262-121">例如, 基于类型:</span><span class="sxs-lookup"><span data-stu-id="02262-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="02262-122">或基于容器类型:</span><span class="sxs-lookup"><span data-stu-id="02262-122">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="02262-123">请参阅可在[resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="02262-123">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="02262-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="02262-124">Request headers</span></span>
| <span data-ttu-id="02262-125">标头</span><span class="sxs-lookup"><span data-stu-id="02262-125">Header</span></span>       |  <span data-ttu-id="02262-126">值</span><span class="sxs-lookup"><span data-stu-id="02262-126">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="02262-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="02262-127">Authorization</span></span>  | <span data-ttu-id="02262-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="02262-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="02262-130">接受</span><span class="sxs-lookup"><span data-stu-id="02262-130">Accept</span></span>  | <span data-ttu-id="02262-131">application/json</span><span class="sxs-lookup"><span data-stu-id="02262-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02262-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="02262-132">Request body</span></span>
<span data-ttu-id="02262-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02262-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02262-134">响应</span><span class="sxs-lookup"><span data-stu-id="02262-134">Response</span></span>

<span data-ttu-id="02262-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和已[使用](../resources/insights-used.md)项的列表。</span><span class="sxs-lookup"><span data-stu-id="02262-135">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02262-136">示例</span><span class="sxs-lookup"><span data-stu-id="02262-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="02262-137">请求</span><span class="sxs-lookup"><span data-stu-id="02262-137">Request</span></span>

<span data-ttu-id="02262-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="02262-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="02262-139">响应</span><span class="sxs-lookup"><span data-stu-id="02262-139">Response</span></span>

<span data-ttu-id="02262-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="02262-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

### <a name="expanding-resource"></a><span data-ttu-id="02262-143">扩展资源</span><span class="sxs-lookup"><span data-stu-id="02262-143">Expanding resource</span></span>
<span data-ttu-id="02262-144">可以扩展已使用的洞察力引用的资源。</span><span class="sxs-lookup"><span data-stu-id="02262-144">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
