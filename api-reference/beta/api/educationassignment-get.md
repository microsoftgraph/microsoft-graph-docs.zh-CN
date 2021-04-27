---
title: 获取 educationAssignment
description: " 教师可以看到课程的所有作业。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 33d08133c289402cbc4eec1ce4775cf710c58582
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044422"
---
# <a name="get-educationassignment"></a><span data-ttu-id="83260-103">获取 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="83260-103">Get educationAssignment</span></span>

<span data-ttu-id="83260-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83260-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83260-105">获取工作分配的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83260-105">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="83260-106">学生只能看到分配给他们的作业;教师和具有应用程序权限的应用程序可以看到课程的所有作业。</span><span class="sxs-lookup"><span data-stu-id="83260-106">Students can only see assignments assigned to them; teachers and applications with application permissions can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="83260-107">权限</span><span class="sxs-lookup"><span data-stu-id="83260-107">Permissions</span></span>
<span data-ttu-id="83260-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83260-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="83260-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="83260-110">Permission type</span></span>      | <span data-ttu-id="83260-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83260-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83260-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83260-112">Delegated (work or school account)</span></span> | <span data-ttu-id="83260-113">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83260-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="83260-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83260-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="83260-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="83260-115">Not supported.</span></span>  |
|<span data-ttu-id="83260-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="83260-116">Application</span></span> | <span data-ttu-id="83260-117">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83260-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="83260-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83260-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83260-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="83260-119">Optional query parameters</span></span>
<span data-ttu-id="83260-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="83260-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83260-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="83260-121">Request headers</span></span>
| <span data-ttu-id="83260-122">标头</span><span class="sxs-lookup"><span data-stu-id="83260-122">Header</span></span>       | <span data-ttu-id="83260-123">值</span><span class="sxs-lookup"><span data-stu-id="83260-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83260-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="83260-124">Authorization</span></span>  | <span data-ttu-id="83260-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83260-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83260-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="83260-127">Request body</span></span>
<span data-ttu-id="83260-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="83260-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83260-129">响应</span><span class="sxs-lookup"><span data-stu-id="83260-129">Response</span></span>
<span data-ttu-id="83260-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationAssignment](../resources/educationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83260-130">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83260-131">示例</span><span class="sxs-lookup"><span data-stu-id="83260-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83260-132">请求</span><span class="sxs-lookup"><span data-stu-id="83260-132">Request</span></span>
<span data-ttu-id="83260-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="83260-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83260-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="83260-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="c"></a>[<span data-ttu-id="83260-135">C#</span><span class="sxs-lookup"><span data-stu-id="83260-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83260-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83260-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83260-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83260-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83260-138">Java</span><span class="sxs-lookup"><span data-stu-id="83260-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="83260-139">响应</span><span class="sxs-lookup"><span data-stu-id="83260-139">Response</span></span>
<span data-ttu-id="83260-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="83260-140">The following is an example of the response.</span></span> 

><span data-ttu-id="83260-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="83260-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
