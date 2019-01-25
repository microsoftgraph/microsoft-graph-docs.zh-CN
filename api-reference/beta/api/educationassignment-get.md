---
title: 获取 educationAssignment
description: " 教师可以查看类中的所有工作分配。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: eba959dcaf2478f3c49fc0fbb434d7269e37e5ba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508368"
---
# <a name="get-educationassignment"></a><span data-ttu-id="11448-103">获取 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="11448-103">Get educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11448-104">要获取的属性和工作分配的关系。</span><span class="sxs-lookup"><span data-stu-id="11448-104">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="11448-105">学生只能看到分配分配给它们。教师可以查看类中的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="11448-105">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="11448-106">权限</span><span class="sxs-lookup"><span data-stu-id="11448-106">Permissions</span></span>
<span data-ttu-id="11448-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11448-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="11448-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="11448-109">Permission type</span></span>      | <span data-ttu-id="11448-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11448-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11448-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11448-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11448-112">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11448-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="11448-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11448-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="11448-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="11448-114">Not supported.</span></span>  |
|<span data-ttu-id="11448-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="11448-115">Application</span></span> | <span data-ttu-id="11448-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="11448-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="11448-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11448-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="11448-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="11448-118">Optional query parameters</span></span>
<span data-ttu-id="11448-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="11448-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11448-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="11448-120">Request headers</span></span>
| <span data-ttu-id="11448-121">标头</span><span class="sxs-lookup"><span data-stu-id="11448-121">Header</span></span>       | <span data-ttu-id="11448-122">值</span><span class="sxs-lookup"><span data-stu-id="11448-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="11448-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11448-123">Authorization</span></span>  | <span data-ttu-id="11448-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11448-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11448-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="11448-126">Request body</span></span>
<span data-ttu-id="11448-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="11448-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11448-128">响应</span><span class="sxs-lookup"><span data-stu-id="11448-128">Response</span></span>
<span data-ttu-id="11448-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationAssignment](../resources/educationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="11448-129">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="11448-130">示例</span><span class="sxs-lookup"><span data-stu-id="11448-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11448-131">请求</span><span class="sxs-lookup"><span data-stu-id="11448-131">Request</span></span>
<span data-ttu-id="11448-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="11448-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="11448-133">响应</span><span class="sxs-lookup"><span data-stu-id="11448-133">Response</span></span>
<span data-ttu-id="11448-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="11448-134">The following is an example of the response.</span></span> 

><span data-ttu-id="11448-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="11448-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
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
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
