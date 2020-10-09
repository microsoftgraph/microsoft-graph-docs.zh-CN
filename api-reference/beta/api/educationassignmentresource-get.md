---
title: 获取 educationAssignmentResource
description: '获取工作分配的特定资源的属性。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a60e52ca35630640685123288013c7d396462341
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403585"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="0d7fa-103">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="0d7fa-103">Get educationAssignmentResource</span></span>

<span data-ttu-id="0d7fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d7fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d7fa-105">获取工作分配的特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-105">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="0d7fa-106">权限</span><span class="sxs-lookup"><span data-stu-id="0d7fa-106">Permissions</span></span>
<span data-ttu-id="0d7fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d7fa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d7fa-109">Permission type</span></span>      | <span data-ttu-id="0d7fa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d7fa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d7fa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d7fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d7fa-112">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="0d7fa-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="0d7fa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d7fa-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0d7fa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-114">Not supported.</span></span>  |
|<span data-ttu-id="0d7fa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d7fa-115">Application</span></span> |  <span data-ttu-id="0d7fa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0d7fa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d7fa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0d7fa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0d7fa-118">Optional query parameters</span></span>
<span data-ttu-id="0d7fa-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d7fa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d7fa-120">Request headers</span></span>
| <span data-ttu-id="0d7fa-121">标头</span><span class="sxs-lookup"><span data-stu-id="0d7fa-121">Header</span></span>       | <span data-ttu-id="0d7fa-122">值</span><span class="sxs-lookup"><span data-stu-id="0d7fa-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d7fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d7fa-123">Authorization</span></span>  | <span data-ttu-id="0d7fa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d7fa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d7fa-126">Request body</span></span>
<span data-ttu-id="0d7fa-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0d7fa-128">响应</span><span class="sxs-lookup"><span data-stu-id="0d7fa-128">Response</span></span>
<span data-ttu-id="0d7fa-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-129">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d7fa-130">示例</span><span class="sxs-lookup"><span data-stu-id="0d7fa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d7fa-131">请求</span><span class="sxs-lookup"><span data-stu-id="0d7fa-131">Request</span></span>
<span data-ttu-id="0d7fa-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d7fa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d7fa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="0d7fa-134">C#</span><span class="sxs-lookup"><span data-stu-id="0d7fa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d7fa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d7fa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d7fa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d7fa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0d7fa-137">响应</span><span class="sxs-lookup"><span data-stu-id="0d7fa-137">Response</span></span>
<span data-ttu-id="0d7fa-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-138">The following is an example of the response.</span></span> 

><span data-ttu-id="0d7fa-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0d7fa-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0d7fa-140">All of the properties will be returned from an actual call.</span></span>

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