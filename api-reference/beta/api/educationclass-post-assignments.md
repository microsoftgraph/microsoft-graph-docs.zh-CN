---
title: 创建 educationAssignment
description: '创建新的工作分配。 只有课堂中的教师才能创建作业。 作业以草稿状态开始，这意味着在调用发布之前，学生不会看到作业。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 399f97fc7e93657f7c3eefb039f5a410121e7a65
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470227"
---
# <a name="create-educationassignment"></a><span data-ttu-id="086fe-105">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="086fe-105">Create educationAssignment</span></span>

<span data-ttu-id="086fe-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="086fe-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="086fe-107">创建新的工作分配。</span><span class="sxs-lookup"><span data-stu-id="086fe-107">Creates a new assignment.</span></span> <span data-ttu-id="086fe-108">只有课堂中的教师才能创建作业。</span><span class="sxs-lookup"><span data-stu-id="086fe-108">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="086fe-109">作业以草稿状态开始，这意味着在调用发布之前，学生不会看到作业。</span><span class="sxs-lookup"><span data-stu-id="086fe-109">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="086fe-110">权限</span><span class="sxs-lookup"><span data-stu-id="086fe-110">Permissions</span></span>
<span data-ttu-id="086fe-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="086fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="086fe-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="086fe-113">Permission type</span></span>      | <span data-ttu-id="086fe-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="086fe-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="086fe-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="086fe-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="086fe-116">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="086fe-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="086fe-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="086fe-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="086fe-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="086fe-118">Not supported.</span></span>  |
|<span data-ttu-id="086fe-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="086fe-119">Application</span></span> | <span data-ttu-id="086fe-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="086fe-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="086fe-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="086fe-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments
```
## <a name="request-headers"></a><span data-ttu-id="086fe-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="086fe-122">Request headers</span></span>
| <span data-ttu-id="086fe-123">标头</span><span class="sxs-lookup"><span data-stu-id="086fe-123">Header</span></span>       | <span data-ttu-id="086fe-124">值</span><span class="sxs-lookup"><span data-stu-id="086fe-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="086fe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="086fe-125">Authorization</span></span>  | <span data-ttu-id="086fe-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="086fe-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="086fe-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="086fe-128">Content-Type</span></span>  | <span data-ttu-id="086fe-129">application/json</span><span class="sxs-lookup"><span data-stu-id="086fe-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="086fe-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="086fe-130">Request body</span></span>
<span data-ttu-id="086fe-131">在请求正文中，提供 [educationAssignment](../resources/educationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="086fe-131">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="086fe-132">响应</span><span class="sxs-lookup"><span data-stu-id="086fe-132">Response</span></span>
<span data-ttu-id="086fe-133">如果成功，此方法在响应正文中返回响应 `201 Created` 代码和 [educationAssignment](../resources/educationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="086fe-133">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="086fe-134">示例</span><span class="sxs-lookup"><span data-stu-id="086fe-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="086fe-135">请求</span><span class="sxs-lookup"><span data-stu-id="086fe-135">Request</span></span>
<span data-ttu-id="086fe-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="086fe-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignment_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11019/assignments
Content-type: application/json
Content-length: 279

{ 
  "dueDateTime": "2014-02-01T00:00:00Z",
  "displayName": "Midterm 1",
    "instructions":  {
      "contentType": "text",
      "content": "Read chapters 1 through 3"
    },
      "grading": {
        "@odata.type": "#microsoft.education.assignments.api.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "assignTo": {
        "@odata.type": "#microsoft.education.assignments.api.educationAssignmentClassRecipient"
      },
      "status":"draft",
      "allowStudentsToAddResourcesToSubmission": true
}
```
<span data-ttu-id="086fe-137">在请求正文中，提供 [educationAssignment](../resources/educationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="086fe-137">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="086fe-138">响应</span><span class="sxs-lookup"><span data-stu-id="086fe-138">Response</span></span>
<span data-ttu-id="086fe-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="086fe-139">The following is an example of the response.</span></span> 

><span data-ttu-id="086fe-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="086fe-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 279

{
  "addedStudentAction": "none",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "2014-02-01T00:00:00Z",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-02-01T00:00:00Z",
  "classId": "11018",
  "closeDateTime": "2014-02-11T00:00:00Z",
  "createdBy": {
      "application": null,
      "device": null,
      "user": {
          "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
          "displayName": null
      }
  },
  "createdDateTime": "2014-02-01T00:00:00Z",
  "displayName": "published",
  "dueDateTime": "2014-02-01T00:00:00Z",
  "grading": {
    "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
    "maxPoints": 100
  },
  "instructions": {
    "contentType": "text",
    "content": "Read chapters 1 through 3"
  },
  "lastModifiedBy": {
      "application": null,
      "device": null,
      "user": {
          "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
          "displayName": null
      }
  },
  "lastModifiedDateTime": "2014-02-01T00:00:00Z",
  "notificationChannelUrl": null,
  "status": "published"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


