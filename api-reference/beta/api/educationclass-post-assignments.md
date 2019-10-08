---
title: 创建 educationAssignment
description: '创建新的工作分配。 只有课堂中的教师才能创建工作分配。 工作分配从草稿状态开始，这意味着在调用 publish 之前，学生将看不到分配。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2fe916bf7b37e7c7ee2e0487185b585075fd32cc
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418228"
---
# <a name="create-educationassignment"></a><span data-ttu-id="da40d-105">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="da40d-105">Create educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da40d-106">创建新的工作分配。</span><span class="sxs-lookup"><span data-stu-id="da40d-106">Creates a new assignment.</span></span> <span data-ttu-id="da40d-107">只有课堂中的教师才能创建工作分配。</span><span class="sxs-lookup"><span data-stu-id="da40d-107">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="da40d-108">工作分配从草稿状态开始，这意味着在调用 publish 之前，学生将看不到分配。</span><span class="sxs-lookup"><span data-stu-id="da40d-108">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="da40d-109">权限</span><span class="sxs-lookup"><span data-stu-id="da40d-109">Permissions</span></span>
<span data-ttu-id="da40d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da40d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da40d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="da40d-112">Permission type</span></span>      | <span data-ttu-id="da40d-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da40d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da40d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da40d-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="da40d-115">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="da40d-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="da40d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da40d-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="da40d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="da40d-117">Not supported.</span></span>  |
|<span data-ttu-id="da40d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="da40d-118">Application</span></span> | <span data-ttu-id="da40d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="da40d-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="da40d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da40d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="da40d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="da40d-121">Request headers</span></span>
| <span data-ttu-id="da40d-122">标头</span><span class="sxs-lookup"><span data-stu-id="da40d-122">Header</span></span>       | <span data-ttu-id="da40d-123">值</span><span class="sxs-lookup"><span data-stu-id="da40d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da40d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="da40d-124">Authorization</span></span>  | <span data-ttu-id="da40d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="da40d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da40d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da40d-127">Content-Type</span></span>  | <span data-ttu-id="da40d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da40d-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da40d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="da40d-129">Request body</span></span>
<span data-ttu-id="da40d-130">在请求正文中，提供[educationAssignment](../resources/educationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da40d-130">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="da40d-131">响应</span><span class="sxs-lookup"><span data-stu-id="da40d-131">Response</span></span>
<span data-ttu-id="da40d-132">如果成功，此方法在响应`201 Created`正文中返回响应代码和[educationAssignment](../resources/educationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da40d-132">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da40d-133">示例</span><span class="sxs-lookup"><span data-stu-id="da40d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da40d-134">请求</span><span class="sxs-lookup"><span data-stu-id="da40d-134">Request</span></span>
<span data-ttu-id="da40d-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="da40d-135">The following is an example of the request.</span></span>
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
<span data-ttu-id="da40d-136">在请求正文中，提供[educationAssignment](../resources/educationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da40d-136">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="da40d-137">响应</span><span class="sxs-lookup"><span data-stu-id="da40d-137">Response</span></span>
<span data-ttu-id="da40d-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="da40d-138">The following is an example of the response.</span></span> 

><span data-ttu-id="da40d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="da40d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 279

{
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
