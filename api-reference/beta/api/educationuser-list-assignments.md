---
title: 列表分配
description: 返回分配给用户的所有类的分配的列表。 此实用程序命名空间允许呼叫者可以在单个呼叫，而不必重新分配请求从每个类中查找学生的所有工作分配。 工作分配列表包含所需获取类命名空间内从工作分配的详细的信息。 工作分配的所有其他操作应使用类命名空间。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e2e11eb94c07fc523d6d64143ffc3df401fd9906
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515977"
---
# <a name="list-assignments"></a><span data-ttu-id="937ed-106">列表分配</span><span class="sxs-lookup"><span data-stu-id="937ed-106">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="937ed-107">返回分配给用户的所有类的分配的列表。</span><span class="sxs-lookup"><span data-stu-id="937ed-107">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="937ed-108">此实用程序命名空间允许呼叫者可以在单个呼叫，而不必重新分配请求从每个类中查找学生的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="937ed-108">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="937ed-109">工作分配列表包含所需获取类命名空间内从工作分配的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="937ed-109">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="937ed-110">工作分配的所有其他操作应使用类命名空间。</span><span class="sxs-lookup"><span data-stu-id="937ed-110">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="937ed-111">权限</span><span class="sxs-lookup"><span data-stu-id="937ed-111">Permissions</span></span>
<span data-ttu-id="937ed-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="937ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="937ed-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="937ed-114">Permission type</span></span>      | <span data-ttu-id="937ed-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="937ed-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="937ed-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="937ed-116">Delegated (work or school account)</span></span> | <span data-ttu-id="937ed-117">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="937ed-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="937ed-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="937ed-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="937ed-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="937ed-119">Not supported.</span></span>   |
|<span data-ttu-id="937ed-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="937ed-120">Application</span></span> | <span data-ttu-id="937ed-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="937ed-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="937ed-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="937ed-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="937ed-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="937ed-123">Optional query parameters</span></span>
<span data-ttu-id="937ed-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="937ed-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="937ed-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="937ed-125">Request headers</span></span>
| <span data-ttu-id="937ed-126">标头</span><span class="sxs-lookup"><span data-stu-id="937ed-126">Header</span></span>       | <span data-ttu-id="937ed-127">值</span><span class="sxs-lookup"><span data-stu-id="937ed-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="937ed-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="937ed-128">Authorization</span></span>  | <span data-ttu-id="937ed-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="937ed-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="937ed-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="937ed-131">Request body</span></span>
<span data-ttu-id="937ed-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="937ed-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="937ed-133">响应</span><span class="sxs-lookup"><span data-stu-id="937ed-133">Response</span></span>
<span data-ttu-id="937ed-134">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationAssignment](../resources/educationassignment.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="937ed-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="937ed-135">示例</span><span class="sxs-lookup"><span data-stu-id="937ed-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="937ed-136">请求</span><span class="sxs-lookup"><span data-stu-id="937ed-136">Request</span></span>
<span data-ttu-id="937ed-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="937ed-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```
##### <a name="response"></a><span data-ttu-id="937ed-138">响应</span><span class="sxs-lookup"><span data-stu-id="937ed-138">Response</span></span>
<span data-ttu-id="937ed-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="937ed-139">The following is an example of the response.</span></span> 

><span data-ttu-id="937ed-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="937ed-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
  "value": [
    {
      "id": "19002",
      "allowLateSubmissions": true,
      "allowStudentsToAddResourcesToSubmission": true,
      "assignDateTime": "2014-01-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-01-01T00:00:00Z",
      "classId": "11010",
      "createdBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "createdDateTime": "2014-01-01T00:00:00Z",
      "displayName": "Assignment 1",
      "dueDateTime": "2014-01-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "content": "Answer every question correctly",
        "contentType": "Text"
      },
      "lastModifiedBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "lastModifiedDateTime": "2014-01-01T00:00:00Z",
      "status": "assigned"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationuser-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
