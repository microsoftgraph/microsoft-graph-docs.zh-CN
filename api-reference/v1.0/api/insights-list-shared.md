---
title: 共享的列表
description: 计算得出的见解，可返回与用户共享的文件列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 8aa3267de5373e0f75f73851c4d995cbb29cd8bf
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844347"
---
# <a name="list-shared"></a><span data-ttu-id="9648e-103">共享的列表</span><span class="sxs-lookup"><span data-stu-id="9648e-103">List shared</span></span>

<span data-ttu-id="9648e-104">计算的洞察力，包括与用户共享的文档列表。</span><span class="sxs-lookup"><span data-stu-id="9648e-104">Calculated insight that includes the list of documents shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9648e-105">权限</span><span class="sxs-lookup"><span data-stu-id="9648e-105">Permissions</span></span>
<span data-ttu-id="9648e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9648e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9648e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9648e-108">Permission type</span></span>      | <span data-ttu-id="9648e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9648e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9648e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9648e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9648e-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9648e-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9648e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9648e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9648e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9648e-113">Not supported.</span></span>    |
|<span data-ttu-id="9648e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9648e-114">Application</span></span> | <span data-ttu-id="9648e-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9648e-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9648e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9648e-116">HTTP request</span></span>
<span data-ttu-id="9648e-117">获取与已登录用户共享的文档列表。</span><span class="sxs-lookup"><span data-stu-id="9648e-117">Get a list of documents shared with the signed-in user.</span></span>

><span data-ttu-id="9648e-118">**注意**：只有用户可以使用用户的 id 或主体名称发出请求。</span><span class="sxs-lookup"><span data-stu-id="9648e-118">**Note**: Only the user can make requests using the user's id or principal name.</span></span>

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

<span data-ttu-id="9648e-119">扩展**共享**洞察力引用的资源：</span><span class="sxs-lookup"><span data-stu-id="9648e-119">Expand the resource referenced by a **shared** insight:</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9648e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9648e-120">Optional query parameters</span></span>
<span data-ttu-id="9648e-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9648e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="9648e-122">您可以使用`$filter`查询参数筛选共享项目。</span><span class="sxs-lookup"><span data-stu-id="9648e-122">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="9648e-123">例如，基于**类型**：</span><span class="sxs-lookup"><span data-stu-id="9648e-123">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="9648e-124">请参阅可在[resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="9648e-124">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="9648e-125">您还可以检索由特定用户共享的文件。</span><span class="sxs-lookup"><span data-stu-id="9648e-125">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="9648e-126">例如，通过指定`lastshared/sharedby/address`属性：</span><span class="sxs-lookup"><span data-stu-id="9648e-126">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="9648e-127">请参阅[sharingDetail](../resources/insights-sharingdetail.md)复杂类型。</span><span class="sxs-lookup"><span data-stu-id="9648e-127">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="9648e-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="9648e-128">Request headers</span></span>
| <span data-ttu-id="9648e-129">标头</span><span class="sxs-lookup"><span data-stu-id="9648e-129">Header</span></span>       |  <span data-ttu-id="9648e-130">值</span><span class="sxs-lookup"><span data-stu-id="9648e-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="9648e-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="9648e-131">Authorization</span></span>  | <span data-ttu-id="9648e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9648e-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9648e-134">接受</span><span class="sxs-lookup"><span data-stu-id="9648e-134">Accept</span></span>  | <span data-ttu-id="9648e-135">application/json</span><span class="sxs-lookup"><span data-stu-id="9648e-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9648e-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="9648e-136">Request body</span></span>
<span data-ttu-id="9648e-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9648e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9648e-138">响应</span><span class="sxs-lookup"><span data-stu-id="9648e-138">Response</span></span>

<span data-ttu-id="9648e-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和[共享](../resources/insights-shared.md)项列表。</span><span class="sxs-lookup"><span data-stu-id="9648e-139">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9648e-140">示例</span><span class="sxs-lookup"><span data-stu-id="9648e-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9648e-141">请求</span><span class="sxs-lookup"><span data-stu-id="9648e-141">Request</span></span>

<span data-ttu-id="9648e-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9648e-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="9648e-143">响应</span><span class="sxs-lookup"><span data-stu-id="9648e-143">Response</span></span>

<span data-ttu-id="9648e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9648e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

