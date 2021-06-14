---
title: 创建 educationAssignment
description: 创建新工作分配。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c169fd1c50f954c47157c480b0c496650b3b233d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911396"
---
# <a name="create-educationassignment"></a><span data-ttu-id="e0409-103">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="e0409-103">Create educationAssignment</span></span>

<span data-ttu-id="e0409-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0409-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0409-105">创建新的工作分配。</span><span class="sxs-lookup"><span data-stu-id="e0409-105">Creates a new assignment.</span></span> 

<span data-ttu-id="e0409-106">只有班级中的教师才能创建作业。</span><span class="sxs-lookup"><span data-stu-id="e0409-106">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="e0409-107">作业从"草稿"状态开始，这意味着学生在发布之前不会看到作业。</span><span class="sxs-lookup"><span data-stu-id="e0409-107">Assignments start in the Draft state, which means that students will not see the assignment until publication.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e0409-108">权限</span><span class="sxs-lookup"><span data-stu-id="e0409-108">Permissions</span></span>
<span data-ttu-id="e0409-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0409-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0409-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0409-111">Permission type</span></span>      | <span data-ttu-id="e0409-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0409-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0409-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0409-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e0409-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0409-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e0409-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0409-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e0409-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0409-116">Not supported.</span></span>  |
|<span data-ttu-id="e0409-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0409-117">Application</span></span> | <span data-ttu-id="e0409-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0409-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e0409-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0409-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments
```
## <a name="request-headers"></a><span data-ttu-id="e0409-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0409-120">Request headers</span></span>
| <span data-ttu-id="e0409-121">标头</span><span class="sxs-lookup"><span data-stu-id="e0409-121">Header</span></span>       | <span data-ttu-id="e0409-122">值</span><span class="sxs-lookup"><span data-stu-id="e0409-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0409-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0409-123">Authorization</span></span>  | <span data-ttu-id="e0409-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0409-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e0409-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0409-126">Content-Type</span></span>  | <span data-ttu-id="e0409-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e0409-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0409-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0409-128">Request body</span></span>
<span data-ttu-id="e0409-129">在请求正文中，提供 [educationAssignment](../resources/educationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0409-129">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0409-130">响应</span><span class="sxs-lookup"><span data-stu-id="e0409-130">Response</span></span>
<span data-ttu-id="e0409-131">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [educationAssignment](../resources/educationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0409-131">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0409-132">示例</span><span class="sxs-lookup"><span data-stu-id="e0409-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0409-133">请求</span><span class="sxs-lookup"><span data-stu-id="e0409-133">Request</span></span>
<span data-ttu-id="e0409-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0409-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationassignment_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/8ddcac47-0b45-4cdb-b10a-d36a07a3dd62/assignments
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
        "@odata.type": "educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "assignTo": {
        "@odata.type": "educationAssignmentClassRecipient"
      },
      "status":"draft",
      "allowStudentsToAddResourcesToSubmission": true
}
```
<span data-ttu-id="e0409-135">在请求正文中，提供 [educationAssignment](../resources/educationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0409-135">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="e0409-136">响应</span><span class="sxs-lookup"><span data-stu-id="e0409-136">Response</span></span>
<span data-ttu-id="e0409-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0409-137">The following is an example of the response.</span></span> 

><span data-ttu-id="e0409-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0409-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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


