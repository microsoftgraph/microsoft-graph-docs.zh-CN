---
title: 使用列表
description: 返回与用户使用的文件列表的计算的洞察。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: e73536d5933d6293539eb00ba8cdc2e85ce5fa93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526100"
---
# <a name="list-used"></a><span data-ttu-id="8541b-103">使用列表</span><span class="sxs-lookup"><span data-stu-id="8541b-103">List used</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8541b-104">返回与用户使用的文件列表的计算的洞察。</span><span class="sxs-lookup"><span data-stu-id="8541b-104">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="8541b-105">权限</span><span class="sxs-lookup"><span data-stu-id="8541b-105">Permissions</span></span>
<span data-ttu-id="8541b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8541b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8541b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8541b-108">Permission type</span></span>      | <span data-ttu-id="8541b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8541b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8541b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8541b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8541b-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8541b-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8541b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8541b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8541b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8541b-113">Not supported.</span></span>    |
|<span data-ttu-id="8541b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8541b-114">Application</span></span> | <span data-ttu-id="8541b-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8541b-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8541b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8541b-116">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="8541b-117">请求其他用户使用的文档返回结果按 lastModifiedDateTime' 和 'lastAccessedDateTime 设置为 lastModifiedDateTime。</span><span class="sxs-lookup"><span data-stu-id="8541b-117">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8541b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8541b-118">Optional query parameters</span></span>
<span data-ttu-id="8541b-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8541b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="8541b-120">您可以使用`$filter`查询参数使用筛选器的项目。</span><span class="sxs-lookup"><span data-stu-id="8541b-120">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="8541b-121">例如，基于类型：</span><span class="sxs-lookup"><span data-stu-id="8541b-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="8541b-122">还是基于容器类型：</span><span class="sxs-lookup"><span data-stu-id="8541b-122">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="8541b-123">请参阅可用的容器类型和[resourceVisualization](../resources/insights-resourcevisualization.md)中可以通过筛选的类型。</span><span class="sxs-lookup"><span data-stu-id="8541b-123">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="8541b-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="8541b-124">Request headers</span></span>
| <span data-ttu-id="8541b-125">标头</span><span class="sxs-lookup"><span data-stu-id="8541b-125">Header</span></span>       |  <span data-ttu-id="8541b-126">值</span><span class="sxs-lookup"><span data-stu-id="8541b-126">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="8541b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8541b-127">Authorization</span></span>  | <span data-ttu-id="8541b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8541b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8541b-130">Accept</span><span class="sxs-lookup"><span data-stu-id="8541b-130">Accept</span></span>  | <span data-ttu-id="8541b-131">application/json</span><span class="sxs-lookup"><span data-stu-id="8541b-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8541b-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="8541b-132">Request body</span></span>
<span data-ttu-id="8541b-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8541b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8541b-134">响应</span><span class="sxs-lookup"><span data-stu-id="8541b-134">Response</span></span>

<span data-ttu-id="8541b-135">如果成功，此方法返回`200 OK`响应代码以及响应正文中[使用](../resources/insights-used.md)项目的列表。</span><span class="sxs-lookup"><span data-stu-id="8541b-135">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8541b-136">示例</span><span class="sxs-lookup"><span data-stu-id="8541b-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8541b-137">请求</span><span class="sxs-lookup"><span data-stu-id="8541b-137">Request</span></span>

<span data-ttu-id="8541b-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8541b-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="8541b-139">响应</span><span class="sxs-lookup"><span data-stu-id="8541b-139">Response</span></span>

<span data-ttu-id="8541b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8541b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

### <a name="expanding-resource"></a><span data-ttu-id="8541b-143">展开资源</span><span class="sxs-lookup"><span data-stu-id="8541b-143">Expanding resource</span></span>
<span data-ttu-id="8541b-144">可以扩展使用洞察引用的资源。</span><span class="sxs-lookup"><span data-stu-id="8541b-144">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
