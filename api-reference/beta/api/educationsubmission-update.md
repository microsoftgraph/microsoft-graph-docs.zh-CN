---
title: 更新 educationsubmission
description: 将评分和反馈添加到提交。 只有教师才能执行此操作。 请注意, 基本权限不具有对年级属性的访问权限, 因此无法对年级或反馈进行写入。 此操作不会向学生发布评分和反馈。 教师必须采取显式释放操作, 才能将评分数据返回给学生。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c420d2c6e512d8fed0d713340fea482b0888ca1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464843"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="25dec-107">更新 educationsubmission</span><span class="sxs-lookup"><span data-stu-id="25dec-107">Update educationsubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25dec-108">将评分和反馈添加到提交。</span><span class="sxs-lookup"><span data-stu-id="25dec-108">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="25dec-109">只有教师才能执行此操作。</span><span class="sxs-lookup"><span data-stu-id="25dec-109">Only teachers can perform this operation.</span></span> <span data-ttu-id="25dec-110">请注意, 基本权限不具有对年级属性的访问权限, 因此无法对年级或反馈进行写入。</span><span class="sxs-lookup"><span data-stu-id="25dec-110">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="25dec-111">此操作不会向学生发布评分和反馈。</span><span class="sxs-lookup"><span data-stu-id="25dec-111">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="25dec-112">教师必须采取显式释放操作, 才能将评分数据返回给学生。</span><span class="sxs-lookup"><span data-stu-id="25dec-112">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="25dec-113">权限</span><span class="sxs-lookup"><span data-stu-id="25dec-113">Permissions</span></span>
<span data-ttu-id="25dec-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25dec-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25dec-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="25dec-116">Permission type</span></span>      | <span data-ttu-id="25dec-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25dec-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25dec-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25dec-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="25dec-119">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25dec-119">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="25dec-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25dec-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25dec-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="25dec-121">Not supported.</span></span>   |
|<span data-ttu-id="25dec-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="25dec-122">Application</span></span> | <span data-ttu-id="25dec-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="25dec-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="25dec-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25dec-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="25dec-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="25dec-125">Request headers</span></span>
| <span data-ttu-id="25dec-126">标头</span><span class="sxs-lookup"><span data-stu-id="25dec-126">Header</span></span>       | <span data-ttu-id="25dec-127">值</span><span class="sxs-lookup"><span data-stu-id="25dec-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25dec-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="25dec-128">Authorization</span></span>  | <span data-ttu-id="25dec-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25dec-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25dec-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="25dec-131">Request body</span></span>
<span data-ttu-id="25dec-132">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="25dec-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="25dec-133">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="25dec-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="25dec-134">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="25dec-134">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="25dec-135">属性</span><span class="sxs-lookup"><span data-stu-id="25dec-135">Property</span></span>     | <span data-ttu-id="25dec-136">类型</span><span class="sxs-lookup"><span data-stu-id="25dec-136">Type</span></span>   |<span data-ttu-id="25dec-137">说明</span><span class="sxs-lookup"><span data-stu-id="25dec-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25dec-138">征求</span><span class="sxs-lookup"><span data-stu-id="25dec-138">feedback</span></span>|<span data-ttu-id="25dec-139">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="25dec-139">educationFeedback</span></span>||
|<span data-ttu-id="25dec-140">grade</span><span class="sxs-lookup"><span data-stu-id="25dec-140">grade</span></span>|<span data-ttu-id="25dec-141">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="25dec-141">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="25dec-142">响应</span><span class="sxs-lookup"><span data-stu-id="25dec-142">Response</span></span>
<span data-ttu-id="25dec-143">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[educationSubmission](../resources/educationsubmission.md)对象。</span><span class="sxs-lookup"><span data-stu-id="25dec-143">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25dec-144">示例</span><span class="sxs-lookup"><span data-stu-id="25dec-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25dec-145">请求</span><span class="sxs-lookup"><span data-stu-id="25dec-145">Request</span></span>
<span data-ttu-id="25dec-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="25dec-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_educationsubmission"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7
Content-type: application/json
Content-length: 658

{
  "feedback": {
    "text": {
      "content": "Good work!",
      "contentType": "Text"
    },
    "feedbackDateTime": "2014-01-01T00:00:00Z",
    "feedbackBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
      "@odata.type": "microsoft.graph.identitySet"
    },
    "@odata.type": "microsoft.graph.educationFeedback"
  },
  "grade": {
      "gradedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
      "@odata.type": "microsoft.graph.identitySet"
    },
    "gradedDateTime": "2014-01-01T00:00:00Z",
    "@odata.type": "microsoft.graph.educationAssignmentGrade"
  }
}
```
##### <a name="response"></a><span data-ttu-id="25dec-147">响应</span><span class="sxs-lookup"><span data-stu-id="25dec-147">Response</span></span>
<span data-ttu-id="25dec-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25dec-148">The following is an example of the response.</span></span> 

><span data-ttu-id="25dec-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="25dec-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1217

{
  "feedback": {
    "text": {
      "content": "Good work!",
      "contentType": "Text"
    },
    "feedbackDateTime": "2014-01-01T00:00:00Z",
    "feedbackBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      }
    },
    "@odata.type": "microsoft.graph.educationFeedback"
  },
  "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
          "@odata.type": "microsoft.graph.identitySet"
        },
        "gradedDateTime": "2014-01-01T00:00:00Z",
        "@odata.type": "microsoft.graph.educationAssignmentGrade"
  },
  "id": "850f51b7",
  "recipient": {
    userId:"dsfewsddf",
    "@odata.type": "#microsoft.graph.educationSubmissionRecipient"
  },
  "releasedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    },
  },
  "releasedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "String",
  "status": "completed",
  "submittedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    },
  },
  "submittedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationsubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
