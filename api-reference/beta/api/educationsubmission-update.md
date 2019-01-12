---
title: 更新 educationsubmission
description: 将薪等级和反馈添加到提交。 仅教师可以执行此操作。 请注意，基本权限不具有访问薪等级属性，因此无法写入薪等级或反馈。 此操作不会释放分数，以及向学生发送反馈。 教师必须采取的薪等级数据返回到学生显式释放操作。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7ebe8445a6537333ed17f3626a58258a952ee844
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975335"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="2d92f-107">更新 educationsubmission</span><span class="sxs-lookup"><span data-stu-id="2d92f-107">Update educationsubmission</span></span>

> <span data-ttu-id="2d92f-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2d92f-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d92f-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2d92f-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d92f-110">将薪等级和反馈添加到提交。</span><span class="sxs-lookup"><span data-stu-id="2d92f-110">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="2d92f-111">仅教师可以执行此操作。</span><span class="sxs-lookup"><span data-stu-id="2d92f-111">Only teachers can perform this operation.</span></span> <span data-ttu-id="2d92f-112">请注意，基本权限不具有访问薪等级属性，因此无法写入薪等级或反馈。</span><span class="sxs-lookup"><span data-stu-id="2d92f-112">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="2d92f-113">此操作不会释放分数，以及向学生发送反馈。</span><span class="sxs-lookup"><span data-stu-id="2d92f-113">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="2d92f-114">教师必须采取的薪等级数据返回到学生显式释放操作。</span><span class="sxs-lookup"><span data-stu-id="2d92f-114">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d92f-115">权限</span><span class="sxs-lookup"><span data-stu-id="2d92f-115">Permissions</span></span>
<span data-ttu-id="2d92f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d92f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d92f-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d92f-118">Permission type</span></span>      | <span data-ttu-id="2d92f-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d92f-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d92f-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d92f-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="2d92f-121">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d92f-121">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2d92f-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d92f-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d92f-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d92f-123">Not supported.</span></span>   |
|<span data-ttu-id="2d92f-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d92f-124">Application</span></span> | <span data-ttu-id="2d92f-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d92f-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2d92f-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d92f-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2d92f-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d92f-127">Request headers</span></span>
| <span data-ttu-id="2d92f-128">标头</span><span class="sxs-lookup"><span data-stu-id="2d92f-128">Header</span></span>       | <span data-ttu-id="2d92f-129">值</span><span class="sxs-lookup"><span data-stu-id="2d92f-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d92f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d92f-130">Authorization</span></span>  | <span data-ttu-id="2d92f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d92f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d92f-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d92f-133">Request body</span></span>
<span data-ttu-id="2d92f-134">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="2d92f-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2d92f-135">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2d92f-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2d92f-136">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2d92f-136">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="2d92f-137">属性</span><span class="sxs-lookup"><span data-stu-id="2d92f-137">Property</span></span>     | <span data-ttu-id="2d92f-138">类型</span><span class="sxs-lookup"><span data-stu-id="2d92f-138">Type</span></span>   |<span data-ttu-id="2d92f-139">说明</span><span class="sxs-lookup"><span data-stu-id="2d92f-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d92f-140">反馈</span><span class="sxs-lookup"><span data-stu-id="2d92f-140">feedback</span></span>|<span data-ttu-id="2d92f-141">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="2d92f-141">educationFeedback</span></span>||
|<span data-ttu-id="2d92f-142">grade</span><span class="sxs-lookup"><span data-stu-id="2d92f-142">grade</span></span>|<span data-ttu-id="2d92f-143">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="2d92f-143">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="2d92f-144">响应</span><span class="sxs-lookup"><span data-stu-id="2d92f-144">Response</span></span>
<span data-ttu-id="2d92f-145">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[educationSubmission](../resources/educationsubmission.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d92f-145">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d92f-146">示例</span><span class="sxs-lookup"><span data-stu-id="2d92f-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d92f-147">请求</span><span class="sxs-lookup"><span data-stu-id="2d92f-147">Request</span></span>
<span data-ttu-id="2d92f-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2d92f-148">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2d92f-149">响应</span><span class="sxs-lookup"><span data-stu-id="2d92f-149">Response</span></span>
<span data-ttu-id="2d92f-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2d92f-150">The following is an example of the response.</span></span> 

><span data-ttu-id="2d92f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2d92f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationsubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
