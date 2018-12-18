---
title: 共享列表
description: 返回与用户共享的文件列表中的计算的洞察。
author: simonhult
ms.openlocfilehash: 5d8c4632f2ccb48cc83c3467ddfe0c973f390947
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345813"
---
# <a name="list-shared"></a><span data-ttu-id="b2584-103">共享列表</span><span class="sxs-lookup"><span data-stu-id="b2584-103">List shared</span></span>

> <span data-ttu-id="b2584-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b2584-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2584-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b2584-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2584-106">返回与用户共享的文件列表中的计算的洞察。</span><span class="sxs-lookup"><span data-stu-id="b2584-106">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2584-107">权限</span><span class="sxs-lookup"><span data-stu-id="b2584-107">Permissions</span></span>
<span data-ttu-id="b2584-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2584-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2584-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2584-110">Permission type</span></span>      | <span data-ttu-id="b2584-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2584-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2584-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2584-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b2584-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2584-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2584-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2584-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2584-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2584-115">Not supported.</span></span>    |
|<span data-ttu-id="b2584-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2584-116">Application</span></span> | <span data-ttu-id="b2584-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2584-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2584-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2584-118">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="b2584-119">请求用户 id 或者 userPrincipalName 才可以访问由用户，而不是任何其他人：</span><span class="sxs-lookup"><span data-stu-id="b2584-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2584-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b2584-120">Optional query parameters</span></span>
<span data-ttu-id="b2584-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b2584-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b2584-122">您可以使用`$filter`查询参数来筛选共享的项目。</span><span class="sxs-lookup"><span data-stu-id="b2584-122">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="b2584-123">例如，基于类型：</span><span class="sxs-lookup"><span data-stu-id="b2584-123">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="b2584-124">请参阅可用的容器类型和[resourceVisualization](../resources/insights-resourcevisualization.md)中可以通过筛选的类型。</span><span class="sxs-lookup"><span data-stu-id="b2584-124">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="b2584-125">您还可以检索特定的用户共享的文件。</span><span class="sxs-lookup"><span data-stu-id="b2584-125">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="b2584-126">例如，通过指定`lastshared/sharedby/address`属性：</span><span class="sxs-lookup"><span data-stu-id="b2584-126">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="b2584-127">请参阅[sharingDetail](../resources/insights-sharingdetail.md)复杂类型。</span><span class="sxs-lookup"><span data-stu-id="b2584-127">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="b2584-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2584-128">Request headers</span></span>
| <span data-ttu-id="b2584-129">标头</span><span class="sxs-lookup"><span data-stu-id="b2584-129">Header</span></span>       |  <span data-ttu-id="b2584-130">值</span><span class="sxs-lookup"><span data-stu-id="b2584-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="b2584-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2584-131">Authorization</span></span>  | <span data-ttu-id="b2584-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2584-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b2584-134">Accept</span><span class="sxs-lookup"><span data-stu-id="b2584-134">Accept</span></span>  | <span data-ttu-id="b2584-135">application/json</span><span class="sxs-lookup"><span data-stu-id="b2584-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2584-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2584-136">Request body</span></span>
<span data-ttu-id="b2584-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b2584-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2584-138">响应</span><span class="sxs-lookup"><span data-stu-id="b2584-138">Response</span></span>

<span data-ttu-id="b2584-139">如果成功，此方法返回`200 OK`响应代码以及响应正文中的[共享](../resources/insights-shared.md)项目的列表。</span><span class="sxs-lookup"><span data-stu-id="b2584-139">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b2584-140">示例</span><span class="sxs-lookup"><span data-stu-id="b2584-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b2584-141">请求</span><span class="sxs-lookup"><span data-stu-id="b2584-141">Request</span></span>

<span data-ttu-id="b2584-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2584-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="b2584-143">响应</span><span class="sxs-lookup"><span data-stu-id="b2584-143">Response</span></span>

<span data-ttu-id="b2584-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2584-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="b2584-147">展开资源</span><span class="sxs-lookup"><span data-stu-id="b2584-147">Expanding resource</span></span>
<span data-ttu-id="b2584-148">可以扩展共享洞察引用的资源。</span><span class="sxs-lookup"><span data-stu-id="b2584-148">The resource referenced by a shared insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```