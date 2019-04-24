---
title: 创建 educationAssignment
description: '创建新的工作分配。 只有课堂中的教师才能创建工作分配。 工作分配从草稿状态开始, 这意味着在调用 publish 之前, 学生将看不到分配。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: bac79b8f85eb6141b5159ac5dc7acbf067bf571c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457793"
---
# <a name="create-educationassignment"></a><span data-ttu-id="ab062-105">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="ab062-105">Create educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab062-106">创建新的工作分配。</span><span class="sxs-lookup"><span data-stu-id="ab062-106">Creates a new assignment.</span></span> <span data-ttu-id="ab062-107">只有课堂中的教师才能创建工作分配。</span><span class="sxs-lookup"><span data-stu-id="ab062-107">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="ab062-108">工作分配从草稿状态开始, 这意味着在调用 publish 之前, 学生将看不到分配。</span><span class="sxs-lookup"><span data-stu-id="ab062-108">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="ab062-109">权限</span><span class="sxs-lookup"><span data-stu-id="ab062-109">Permissions</span></span>
<span data-ttu-id="ab062-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab062-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab062-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab062-112">Permission type</span></span>      | <span data-ttu-id="ab062-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab062-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab062-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab062-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="ab062-115">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="ab062-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ab062-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab062-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ab062-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab062-117">Not supported.</span></span>  |
|<span data-ttu-id="ab062-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab062-118">Application</span></span> | <span data-ttu-id="ab062-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab062-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ab062-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab062-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="ab062-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab062-121">Request headers</span></span>
| <span data-ttu-id="ab062-122">标头</span><span class="sxs-lookup"><span data-stu-id="ab062-122">Header</span></span>       | <span data-ttu-id="ab062-123">值</span><span class="sxs-lookup"><span data-stu-id="ab062-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab062-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab062-124">Authorization</span></span>  | <span data-ttu-id="ab062-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab062-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ab062-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab062-127">Content-Type</span></span>  | <span data-ttu-id="ab062-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ab062-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab062-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab062-129">Request body</span></span>
<span data-ttu-id="ab062-130">在请求正文中, 提供[educationAssignment](../resources/educationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab062-130">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ab062-131">响应</span><span class="sxs-lookup"><span data-stu-id="ab062-131">Response</span></span>
<span data-ttu-id="ab062-132">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[educationAssignment](../resources/educationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ab062-132">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab062-133">示例</span><span class="sxs-lookup"><span data-stu-id="ab062-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab062-134">请求</span><span class="sxs-lookup"><span data-stu-id="ab062-134">Request</span></span>
<span data-ttu-id="ab062-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab062-135">The following is an example of the request.</span></span>
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
<span data-ttu-id="ab062-136">在请求正文中, 提供[educationAssignment](../resources/educationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab062-136">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="ab062-137">响应</span><span class="sxs-lookup"><span data-stu-id="ab062-137">Response</span></span>
<span data-ttu-id="ab062-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab062-138">The following is an example of the response.</span></span> 

><span data-ttu-id="ab062-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ab062-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-post-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
