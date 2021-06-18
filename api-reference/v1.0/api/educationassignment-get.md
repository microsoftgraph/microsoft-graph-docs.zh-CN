---
title: 获取 educationAssignment
description: 获取工作分配的属性和关系。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 94f2b3c7854ed650bd262acbac02005a5c8e60bd
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992556"
---
# <a name="get-educationassignment"></a><span data-ttu-id="b683a-103">获取 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="b683a-103">Get educationAssignment</span></span>

<span data-ttu-id="b683a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b683a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b683a-105">获取工作分配的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b683a-105">Get the properties and relationships of an assignment.</span></span> 

<span data-ttu-id="b683a-106">学生只能看到分配给他们的作业;教师和具有应用程序权限的应用程序可以看到课程的所有作业。</span><span class="sxs-lookup"><span data-stu-id="b683a-106">Students can only see assignments assigned to them; teachers and applications with application permissions can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="b683a-107">权限</span><span class="sxs-lookup"><span data-stu-id="b683a-107">Permissions</span></span>
<span data-ttu-id="b683a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b683a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b683a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b683a-110">Permission type</span></span>      | <span data-ttu-id="b683a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b683a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b683a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b683a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b683a-113">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b683a-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="b683a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b683a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b683a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b683a-115">Not supported.</span></span>  |
|<span data-ttu-id="b683a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b683a-116">Application</span></span> | <span data-ttu-id="b683a-117">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b683a-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b683a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b683a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b683a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b683a-119">Optional query parameters</span></span>
<span data-ttu-id="b683a-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b683a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b683a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b683a-121">Request headers</span></span>
| <span data-ttu-id="b683a-122">标头</span><span class="sxs-lookup"><span data-stu-id="b683a-122">Header</span></span>       | <span data-ttu-id="b683a-123">值</span><span class="sxs-lookup"><span data-stu-id="b683a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b683a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b683a-124">Authorization</span></span>  | <span data-ttu-id="b683a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b683a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b683a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b683a-127">Request body</span></span>
<span data-ttu-id="b683a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b683a-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b683a-129">响应</span><span class="sxs-lookup"><span data-stu-id="b683a-129">Response</span></span>
<span data-ttu-id="b683a-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationAssignment](../resources/educationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b683a-130">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b683a-131">示例</span><span class="sxs-lookup"><span data-stu-id="b683a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b683a-132">请求</span><span class="sxs-lookup"><span data-stu-id="b683a-132">Request</span></span>
<span data-ttu-id="b683a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b683a-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b683a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b683a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "get_educationassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/5edb6a5f-fc6b-441b-8952-bcbfc33ef0e5/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0
```
# <a name="c"></a>[<span data-ttu-id="b683a-135">C#</span><span class="sxs-lookup"><span data-stu-id="b683a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b683a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b683a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b683a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b683a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b683a-138">Java</span><span class="sxs-lookup"><span data-stu-id="b683a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b683a-139">响应</span><span class="sxs-lookup"><span data-stu-id="b683a-139">Response</span></span>
<span data-ttu-id="b683a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b683a-140">The following is an example of the response.</span></span> 

><span data-ttu-id="b683a-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b683a-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
  "addedStudentAction": "none",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "classId": "11006",
  "createdBy": {
    "user": {
      "displayName": "Shawn Hughes",
      "id": "14012",
    }
  },
  "closeDateTime": "2014-01-11T00:00:00Z",
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
  "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!0sGAoOieeE6iSj1WXCV-nYYTuh2luKRDvUVGQBLOmvYpRzc5ARnCRorRht6P3MhU/items/01N74NOEZL7P3VK22SQFDKBZ3PHVPKDVAQ",
  "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType",
      "maxPoints": 100
  },
  "instructions": {
    "content": "Answer every question correctly",
    "contentType": "Text"
  },
  "lastModifiedBy": {
    "user": {
      "displayName": "Shawn Hughes",
      "id": "14012",
    }
  },
  "lastModifiedDateTime": "2014-01-01T00:00:00Z",
  "notificationChannelUrl": null,
  "status": "assigned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
