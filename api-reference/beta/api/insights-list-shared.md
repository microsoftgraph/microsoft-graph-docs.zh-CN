---
title: 共享列表
description: 返回与用户共享的文件列表中的计算的洞察。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 2eef2a9b306984a8ad05bcf8fefca2458d609ab1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517349"
---
# <a name="list-shared"></a><span data-ttu-id="4d721-103">共享列表</span><span class="sxs-lookup"><span data-stu-id="4d721-103">List shared</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d721-104">返回与用户共享的文件列表中的计算的洞察。</span><span class="sxs-lookup"><span data-stu-id="4d721-104">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d721-105">权限</span><span class="sxs-lookup"><span data-stu-id="4d721-105">Permissions</span></span>
<span data-ttu-id="4d721-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d721-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d721-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d721-108">Permission type</span></span>      | <span data-ttu-id="4d721-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d721-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d721-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d721-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d721-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d721-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d721-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d721-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d721-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d721-113">Not supported.</span></span>    |
|<span data-ttu-id="4d721-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d721-114">Application</span></span> | <span data-ttu-id="4d721-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d721-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d721-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d721-116">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="4d721-117">请求用户 id 或者 userPrincipalName 才可以访问由用户，而不是任何其他人：</span><span class="sxs-lookup"><span data-stu-id="4d721-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d721-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4d721-118">Optional query parameters</span></span>
<span data-ttu-id="4d721-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4d721-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4d721-120">您可以使用`$filter`查询参数来筛选共享的项目。</span><span class="sxs-lookup"><span data-stu-id="4d721-120">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="4d721-121">例如，基于类型：</span><span class="sxs-lookup"><span data-stu-id="4d721-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="4d721-122">请参阅可用的容器类型和[resourceVisualization](../resources/insights-resourcevisualization.md)中可以通过筛选的类型。</span><span class="sxs-lookup"><span data-stu-id="4d721-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="4d721-123">您还可以检索特定的用户共享的文件。</span><span class="sxs-lookup"><span data-stu-id="4d721-123">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="4d721-124">例如，通过指定`lastshared/sharedby/address`属性：</span><span class="sxs-lookup"><span data-stu-id="4d721-124">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="4d721-125">请参阅[sharingDetail](../resources/insights-sharingdetail.md)复杂类型。</span><span class="sxs-lookup"><span data-stu-id="4d721-125">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="4d721-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d721-126">Request headers</span></span>
| <span data-ttu-id="4d721-127">标头</span><span class="sxs-lookup"><span data-stu-id="4d721-127">Header</span></span>       |  <span data-ttu-id="4d721-128">值</span><span class="sxs-lookup"><span data-stu-id="4d721-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="4d721-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d721-129">Authorization</span></span>  | <span data-ttu-id="4d721-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d721-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4d721-132">Accept</span><span class="sxs-lookup"><span data-stu-id="4d721-132">Accept</span></span>  | <span data-ttu-id="4d721-133">application/json</span><span class="sxs-lookup"><span data-stu-id="4d721-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d721-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d721-134">Request body</span></span>
<span data-ttu-id="4d721-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4d721-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d721-136">响应</span><span class="sxs-lookup"><span data-stu-id="4d721-136">Response</span></span>

<span data-ttu-id="4d721-137">如果成功，此方法返回`200 OK`响应代码以及响应正文中的[共享](../resources/insights-shared.md)项目的列表。</span><span class="sxs-lookup"><span data-stu-id="4d721-137">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d721-138">示例</span><span class="sxs-lookup"><span data-stu-id="4d721-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d721-139">请求</span><span class="sxs-lookup"><span data-stu-id="4d721-139">Request</span></span>

<span data-ttu-id="4d721-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d721-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="4d721-141">响应</span><span class="sxs-lookup"><span data-stu-id="4d721-141">Response</span></span>

<span data-ttu-id="4d721-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d721-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastShared" : { 
                "sharedDateTime" : "sharedDateTime-value",  
                "sharingSubject" : "sharingSubject-value",
                "sharingType" : "sharingType-value", 
                "sharedBy" : { 
                    "displayName" : "displayName-value", 
                    "id": "id-value" 
                }
                "sharingReference" : { 
                    "webUrl" : "webUrl-value",
                    "type: "type-value", 
                    "id": "id-value"
                } 
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
```

### <a name="expanding-resource"></a><span data-ttu-id="4d721-145">展开资源</span><span class="sxs-lookup"><span data-stu-id="4d721-145">Expanding resource</span></span>
<span data-ttu-id="4d721-146">可以扩展共享洞察引用的资源。</span><span class="sxs-lookup"><span data-stu-id="4d721-146">The resource referenced by a shared insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
