---
title: 共享的列表
description: 计算出的洞察力, 返回与用户共享的文件的列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 009d9f65b5403139235e5f9afa932ebbe54ff9d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32500380"
---
# <a name="list-shared"></a><span data-ttu-id="ce2a2-103">共享的列表</span><span class="sxs-lookup"><span data-stu-id="ce2a2-103">List shared</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce2a2-104">计算出的洞察力, 返回与用户共享的文件的列表。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-104">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce2a2-105">权限</span><span class="sxs-lookup"><span data-stu-id="ce2a2-105">Permissions</span></span>
<span data-ttu-id="ce2a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce2a2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce2a2-108">Permission type</span></span>      | <span data-ttu-id="ce2a2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce2a2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce2a2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce2a2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce2a2-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce2a2-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce2a2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce2a2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce2a2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-113">Not supported.</span></span>    |
|<span data-ttu-id="ce2a2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce2a2-114">Application</span></span> | <span data-ttu-id="ce2a2-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce2a2-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce2a2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce2a2-116">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="ce2a2-117">具有 "user id" 或 "userPrincipalName" 的请求只能由用户访问, 而不能由其他人访问:</span><span class="sxs-lookup"><span data-stu-id="ce2a2-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/{id | userPrincipalName}/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce2a2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ce2a2-118">Optional query parameters</span></span>
<span data-ttu-id="ce2a2-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ce2a2-120">您可以使用`$filter`查询参数筛选共享项目。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-120">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="ce2a2-121">例如, 基于类型:</span><span class="sxs-lookup"><span data-stu-id="ce2a2-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="ce2a2-122">请参阅可在[resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="ce2a2-123">您还可以检索由特定用户共享的文件。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-123">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="ce2a2-124">例如, 通过指定`lastshared/sharedby/address`属性:</span><span class="sxs-lookup"><span data-stu-id="ce2a2-124">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="ce2a2-125">请参阅[sharingDetail](../resources/insights-sharingdetail.md)复杂类型。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-125">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ce2a2-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce2a2-126">Request headers</span></span>
| <span data-ttu-id="ce2a2-127">标头</span><span class="sxs-lookup"><span data-stu-id="ce2a2-127">Header</span></span>       |  <span data-ttu-id="ce2a2-128">值</span><span class="sxs-lookup"><span data-stu-id="ce2a2-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="ce2a2-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce2a2-129">Authorization</span></span>  | <span data-ttu-id="ce2a2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ce2a2-132">接受</span><span class="sxs-lookup"><span data-stu-id="ce2a2-132">Accept</span></span>  | <span data-ttu-id="ce2a2-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ce2a2-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce2a2-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce2a2-134">Request body</span></span>
<span data-ttu-id="ce2a2-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce2a2-136">响应</span><span class="sxs-lookup"><span data-stu-id="ce2a2-136">Response</span></span>

<span data-ttu-id="ce2a2-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[共享](../resources/insights-shared.md)项列表。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-137">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce2a2-138">示例</span><span class="sxs-lookup"><span data-stu-id="ce2a2-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ce2a2-139">请求</span><span class="sxs-lookup"><span data-stu-id="ce2a2-139">Request</span></span>

<span data-ttu-id="ce2a2-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="ce2a2-141">响应</span><span class="sxs-lookup"><span data-stu-id="ce2a2-141">Response</span></span>

<span data-ttu-id="ce2a2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="ce2a2-145">扩展资源</span><span class="sxs-lookup"><span data-stu-id="ce2a2-145">Expanding resource</span></span>
<span data-ttu-id="ce2a2-146">共享洞察力引用的资源可以扩展。</span><span class="sxs-lookup"><span data-stu-id="ce2a2-146">The resource referenced by a shared insight can be expanded.</span></span>
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
