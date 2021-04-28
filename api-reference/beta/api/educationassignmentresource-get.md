---
title: 获取 educationAssignmentResource
description: '获取工作分配上特定资源的属性。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f5446926a3161004de1f3a19b5896df95e34ca52
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061684"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="376d3-103">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="376d3-103">Get educationAssignmentResource</span></span>

<span data-ttu-id="376d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="376d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="376d3-105">获取工作分配上特定资源的属性。</span><span class="sxs-lookup"><span data-stu-id="376d3-105">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="376d3-106">权限</span><span class="sxs-lookup"><span data-stu-id="376d3-106">Permissions</span></span>
<span data-ttu-id="376d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="376d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="376d3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="376d3-109">Permission type</span></span>      | <span data-ttu-id="376d3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="376d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="376d3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="376d3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="376d3-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="376d3-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="376d3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="376d3-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="376d3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="376d3-114">Not supported.</span></span>  |
|<span data-ttu-id="376d3-115">Application\*</span><span class="sxs-lookup"><span data-stu-id="376d3-115">Application\*</span></span> |  <span data-ttu-id="376d3-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="376d3-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  | 

<span data-ttu-id="376d3-117">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="376d3-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="376d3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="376d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="376d3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="376d3-119">Optional query parameters</span></span>
<span data-ttu-id="376d3-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="376d3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="376d3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="376d3-121">Request headers</span></span>
| <span data-ttu-id="376d3-122">标头</span><span class="sxs-lookup"><span data-stu-id="376d3-122">Header</span></span>       | <span data-ttu-id="376d3-123">值</span><span class="sxs-lookup"><span data-stu-id="376d3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="376d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="376d3-124">Authorization</span></span>  | <span data-ttu-id="376d3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="376d3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="376d3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="376d3-127">Request body</span></span>
<span data-ttu-id="376d3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="376d3-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="376d3-129">响应</span><span class="sxs-lookup"><span data-stu-id="376d3-129">Response</span></span>
<span data-ttu-id="376d3-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="376d3-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="376d3-131">示例</span><span class="sxs-lookup"><span data-stu-id="376d3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="376d3-132">请求</span><span class="sxs-lookup"><span data-stu-id="376d3-132">Request</span></span>
<span data-ttu-id="376d3-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="376d3-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="376d3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="376d3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="376d3-135">C#</span><span class="sxs-lookup"><span data-stu-id="376d3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="376d3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="376d3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="376d3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="376d3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="376d3-138">Java</span><span class="sxs-lookup"><span data-stu-id="376d3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="376d3-139">响应</span><span class="sxs-lookup"><span data-stu-id="376d3-139">Response</span></span>
<span data-ttu-id="376d3-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="376d3-140">The following is an example of the response.</span></span> 

><span data-ttu-id="376d3-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="376d3-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
