---
title: 获取 educationAssignmentResource
description: '获取工作分配的特定资源的属性。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ce2e8068e164806ecedcb5707938025d86620fd5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416483"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="d7e1e-103">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="d7e1e-103">Get educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7e1e-104">获取工作分配的特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-104">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="d7e1e-105">权限</span><span class="sxs-lookup"><span data-stu-id="d7e1e-105">Permissions</span></span>
<span data-ttu-id="d7e1e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7e1e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7e1e-108">Permission type</span></span>      | <span data-ttu-id="d7e1e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7e1e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7e1e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7e1e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7e1e-111">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="d7e1e-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="d7e1e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7e1e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d7e1e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-113">Not supported.</span></span>  |
|<span data-ttu-id="d7e1e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7e1e-114">Application</span></span> |  <span data-ttu-id="d7e1e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d7e1e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7e1e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7e1e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d7e1e-117">Optional query parameters</span></span>
<span data-ttu-id="d7e1e-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7e1e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7e1e-119">Request headers</span></span>
| <span data-ttu-id="d7e1e-120">标头</span><span class="sxs-lookup"><span data-stu-id="d7e1e-120">Header</span></span>       | <span data-ttu-id="d7e1e-121">值</span><span class="sxs-lookup"><span data-stu-id="d7e1e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d7e1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7e1e-122">Authorization</span></span>  | <span data-ttu-id="d7e1e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7e1e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7e1e-125">Request body</span></span>
<span data-ttu-id="d7e1e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d7e1e-127">响应</span><span class="sxs-lookup"><span data-stu-id="d7e1e-127">Response</span></span>
<span data-ttu-id="d7e1e-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-128">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7e1e-129">示例</span><span class="sxs-lookup"><span data-stu-id="d7e1e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7e1e-130">请求</span><span class="sxs-lookup"><span data-stu-id="d7e1e-130">Request</span></span>
<span data-ttu-id="d7e1e-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d7e1e-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d7e1e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7e1e-133">C#</span><span class="sxs-lookup"><span data-stu-id="d7e1e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7e1e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7e1e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7e1e-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="d7e1e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d7e1e-136">响应</span><span class="sxs-lookup"><span data-stu-id="d7e1e-136">Response</span></span>
<span data-ttu-id="d7e1e-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-137">The following is an example of the response.</span></span> 

><span data-ttu-id="d7e1e-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d7e1e-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7e1e-139">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 842

{
  "distributeForStudentWork": true,
  "id": "22002",
  "resource": {
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "lastModifiedDateTime": "2014-01-01T00:00:00Z"
  }
}
    
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
