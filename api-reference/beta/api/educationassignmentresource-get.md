---
title: 获取 educationAssignmentResource
description: '获取工作分配的特定资源的属性。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4ce38792f2e652c629aa53b0dc4cf5352228e8de
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324182"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="6dec0-103">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="6dec0-103">Get educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dec0-104">获取工作分配的特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="6dec0-104">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="6dec0-105">权限</span><span class="sxs-lookup"><span data-stu-id="6dec0-105">Permissions</span></span>
<span data-ttu-id="6dec0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6dec0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dec0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6dec0-108">Permission type</span></span>      | <span data-ttu-id="6dec0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6dec0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dec0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6dec0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6dec0-111">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="6dec0-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="6dec0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6dec0-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6dec0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dec0-113">Not supported.</span></span>  |
|<span data-ttu-id="6dec0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6dec0-114">Application</span></span> |  <span data-ttu-id="6dec0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dec0-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6dec0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6dec0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6dec0-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6dec0-117">Optional query parameters</span></span>
<span data-ttu-id="6dec0-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6dec0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dec0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6dec0-119">Request headers</span></span>
| <span data-ttu-id="6dec0-120">标头</span><span class="sxs-lookup"><span data-stu-id="6dec0-120">Header</span></span>       | <span data-ttu-id="6dec0-121">值</span><span class="sxs-lookup"><span data-stu-id="6dec0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6dec0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dec0-122">Authorization</span></span>  | <span data-ttu-id="6dec0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6dec0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6dec0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6dec0-125">Request body</span></span>
<span data-ttu-id="6dec0-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6dec0-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6dec0-127">响应</span><span class="sxs-lookup"><span data-stu-id="6dec0-127">Response</span></span>
<span data-ttu-id="6dec0-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6dec0-128">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6dec0-129">示例</span><span class="sxs-lookup"><span data-stu-id="6dec0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6dec0-130">请求</span><span class="sxs-lookup"><span data-stu-id="6dec0-130">Request</span></span>
<span data-ttu-id="6dec0-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6dec0-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6dec0-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6dec0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6dec0-133">C#</span><span class="sxs-lookup"><span data-stu-id="6dec0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6dec0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dec0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6dec0-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="6dec0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6dec0-136">Java</span><span class="sxs-lookup"><span data-stu-id="6dec0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6dec0-137">响应</span><span class="sxs-lookup"><span data-stu-id="6dec0-137">Response</span></span>
<span data-ttu-id="6dec0-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6dec0-138">The following is an example of the response.</span></span> 

><span data-ttu-id="6dec0-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6dec0-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6dec0-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6dec0-140">All of the properties will be returned from an actual call.</span></span>

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
