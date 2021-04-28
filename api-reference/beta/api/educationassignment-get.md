---
title: 获取 educationAssignment
description: " 教师可以看到课程的所有作业。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 28f129d1621be6a54510a8ef1dd4b48e25e2f5ff
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061712"
---
# <a name="get-educationassignment"></a><span data-ttu-id="d8ae6-103">获取 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="d8ae6-103">Get educationAssignment</span></span>

<span data-ttu-id="d8ae6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8ae6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8ae6-105">获取工作分配的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-105">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="d8ae6-106">学生只能看到分配给他们的作业;教师和具有应用程序权限的应用程序可以看到课程的所有作业。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-106">Students can only see assignments assigned to them; teachers and applications with application permissions can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8ae6-107">权限</span><span class="sxs-lookup"><span data-stu-id="d8ae6-107">Permissions</span></span>
<span data-ttu-id="d8ae6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d8ae6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8ae6-110">Permission type</span></span>      | <span data-ttu-id="d8ae6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8ae6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8ae6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8ae6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8ae6-113">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8ae6-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="d8ae6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8ae6-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d8ae6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-115">Not supported.</span></span>  |
|<span data-ttu-id="d8ae6-116">Application\*</span><span class="sxs-lookup"><span data-stu-id="d8ae6-116">Application\*</span></span> | <span data-ttu-id="d8ae6-117">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8ae6-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="d8ae6-118">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-118">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="d8ae6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8ae6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8ae6-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d8ae6-120">Optional query parameters</span></span>
<span data-ttu-id="d8ae6-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8ae6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8ae6-122">Request headers</span></span>
| <span data-ttu-id="d8ae6-123">标头</span><span class="sxs-lookup"><span data-stu-id="d8ae6-123">Header</span></span>       | <span data-ttu-id="d8ae6-124">值</span><span class="sxs-lookup"><span data-stu-id="d8ae6-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8ae6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8ae6-125">Authorization</span></span>  | <span data-ttu-id="d8ae6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8ae6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8ae6-128">Request body</span></span>
<span data-ttu-id="d8ae6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8ae6-130">响应</span><span class="sxs-lookup"><span data-stu-id="d8ae6-130">Response</span></span>
<span data-ttu-id="d8ae6-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationAssignment](../resources/educationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-131">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8ae6-132">示例</span><span class="sxs-lookup"><span data-stu-id="d8ae6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8ae6-133">请求</span><span class="sxs-lookup"><span data-stu-id="d8ae6-133">Request</span></span>
<span data-ttu-id="d8ae6-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8ae6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8ae6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="c"></a>[<span data-ttu-id="d8ae6-136">C#</span><span class="sxs-lookup"><span data-stu-id="d8ae6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8ae6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8ae6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8ae6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8ae6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8ae6-139">Java</span><span class="sxs-lookup"><span data-stu-id="d8ae6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d8ae6-140">响应</span><span class="sxs-lookup"><span data-stu-id="d8ae6-140">Response</span></span>
<span data-ttu-id="d8ae6-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-141">The following is an example of the response.</span></span> 

><span data-ttu-id="d8ae6-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d8ae6-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "closeDateTime": "2014-01-11T00:00:00Z",
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
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
      "displayName": "Susana Rocha",
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
