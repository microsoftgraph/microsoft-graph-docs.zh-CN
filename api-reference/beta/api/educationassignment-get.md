---
title: 获取 educationAssignment
description: " 教师可以查看课程中的所有工作分配。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: df0c4859b650b181ac317374a74093dac7b64353
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325100"
---
# <a name="get-educationassignment"></a><span data-ttu-id="834ca-103">获取 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="834ca-103">Get educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="834ca-104">获取工作分配的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="834ca-104">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="834ca-105">学生只能查看分配给他们的工作分配;教师可以查看课程中的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="834ca-105">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="834ca-106">权限</span><span class="sxs-lookup"><span data-stu-id="834ca-106">Permissions</span></span>
<span data-ttu-id="834ca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="834ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="834ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="834ca-109">Permission type</span></span>      | <span data-ttu-id="834ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="834ca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="834ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="834ca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="834ca-112">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="834ca-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="834ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="834ca-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="834ca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="834ca-114">Not supported.</span></span>  |
|<span data-ttu-id="834ca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="834ca-115">Application</span></span> | <span data-ttu-id="834ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="834ca-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="834ca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="834ca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="834ca-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="834ca-118">Optional query parameters</span></span>
<span data-ttu-id="834ca-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="834ca-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="834ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="834ca-120">Request headers</span></span>
| <span data-ttu-id="834ca-121">标头</span><span class="sxs-lookup"><span data-stu-id="834ca-121">Header</span></span>       | <span data-ttu-id="834ca-122">值</span><span class="sxs-lookup"><span data-stu-id="834ca-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="834ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="834ca-123">Authorization</span></span>  | <span data-ttu-id="834ca-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="834ca-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="834ca-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="834ca-126">Request body</span></span>
<span data-ttu-id="834ca-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="834ca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="834ca-128">响应</span><span class="sxs-lookup"><span data-stu-id="834ca-128">Response</span></span>
<span data-ttu-id="834ca-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationAssignment](../resources/educationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="834ca-129">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="834ca-130">示例</span><span class="sxs-lookup"><span data-stu-id="834ca-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="834ca-131">请求</span><span class="sxs-lookup"><span data-stu-id="834ca-131">Request</span></span>
<span data-ttu-id="834ca-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="834ca-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="834ca-133">响应</span><span class="sxs-lookup"><span data-stu-id="834ca-133">Response</span></span>
<span data-ttu-id="834ca-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="834ca-134">The following is an example of the response.</span></span> 

><span data-ttu-id="834ca-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="834ca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
