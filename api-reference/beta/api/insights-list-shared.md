---
title: 共享的列表
description: 计算得出的见解，可返回与用户共享的文件列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 46d621783540d5521dd04e63f19b3510455a485b
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403036"
---
# <a name="list-shared"></a><span data-ttu-id="8041a-103">共享的列表</span><span class="sxs-lookup"><span data-stu-id="8041a-103">List shared</span></span>

<span data-ttu-id="8041a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8041a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8041a-105">计算的洞察力，包括与用户共享的文档列表。</span><span class="sxs-lookup"><span data-stu-id="8041a-105">Calculated insight that includes the list of documents shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="8041a-106">权限</span><span class="sxs-lookup"><span data-stu-id="8041a-106">Permissions</span></span>
<span data-ttu-id="8041a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8041a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8041a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8041a-109">Permission type</span></span>      | <span data-ttu-id="8041a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8041a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8041a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8041a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8041a-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8041a-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8041a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8041a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8041a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8041a-114">Not supported.</span></span>    |
|<span data-ttu-id="8041a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8041a-115">Application</span></span> | <span data-ttu-id="8041a-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8041a-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8041a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8041a-117">HTTP request</span></span>
<span data-ttu-id="8041a-118">获取与已登录用户共享的文档列表。</span><span class="sxs-lookup"><span data-stu-id="8041a-118">Get a list of documents shared with the signed-in user.</span></span>

><span data-ttu-id="8041a-119">**注意**：只有用户可以使用用户的 id 或主体名称发出请求。</span><span class="sxs-lookup"><span data-stu-id="8041a-119">**Note**: Only the user can make requests using the user's id or principal name.</span></span>

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

<span data-ttu-id="8041a-120">扩展 **共享** 洞察力引用的资源：</span><span class="sxs-lookup"><span data-stu-id="8041a-120">Expand the resource referenced by a **shared** insight:</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8041a-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8041a-121">Optional query parameters</span></span>
<span data-ttu-id="8041a-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8041a-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="8041a-123">您可以使用 `$filter` 查询参数筛选共享项目。</span><span class="sxs-lookup"><span data-stu-id="8041a-123">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="8041a-124">例如，基于 **类型**：</span><span class="sxs-lookup"><span data-stu-id="8041a-124">For example, based on **type**:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="8041a-125">请参阅可在 [resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="8041a-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="8041a-126">您还可以检索由特定用户共享的文件。</span><span class="sxs-lookup"><span data-stu-id="8041a-126">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="8041a-127">例如，通过指定 `lastshared/sharedby/address` 属性：</span><span class="sxs-lookup"><span data-stu-id="8041a-127">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="8041a-128">请参阅 [sharingDetail](../resources/insights-sharingdetail.md) 复杂类型。</span><span class="sxs-lookup"><span data-stu-id="8041a-128">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="8041a-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="8041a-129">Request headers</span></span>
| <span data-ttu-id="8041a-130">标头</span><span class="sxs-lookup"><span data-stu-id="8041a-130">Header</span></span>       |  <span data-ttu-id="8041a-131">值</span><span class="sxs-lookup"><span data-stu-id="8041a-131">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="8041a-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="8041a-132">Authorization</span></span>  | <span data-ttu-id="8041a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8041a-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8041a-135">接受</span><span class="sxs-lookup"><span data-stu-id="8041a-135">Accept</span></span>  | <span data-ttu-id="8041a-136">application/json</span><span class="sxs-lookup"><span data-stu-id="8041a-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8041a-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="8041a-137">Request body</span></span>
<span data-ttu-id="8041a-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8041a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8041a-139">响应</span><span class="sxs-lookup"><span data-stu-id="8041a-139">Response</span></span>

<span data-ttu-id="8041a-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [共享](../resources/insights-shared.md) 项列表。</span><span class="sxs-lookup"><span data-stu-id="8041a-140">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8041a-141">示例</span><span class="sxs-lookup"><span data-stu-id="8041a-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8041a-142">请求</span><span class="sxs-lookup"><span data-stu-id="8041a-142">Request</span></span>

<span data-ttu-id="8041a-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8041a-143">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="8041a-144">响应</span><span class="sxs-lookup"><span data-stu-id="8041a-144">Response</span></span>

<span data-ttu-id="8041a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8041a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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