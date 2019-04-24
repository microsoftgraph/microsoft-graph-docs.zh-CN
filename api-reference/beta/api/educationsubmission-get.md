---
title: 获取 educationSubmission
description: '检索特定的提交。 提交对象表示学生的工作分配。 与提交相关联的资源表示这一工作。 仅向其分配提交的学生可以查看和修改提交。 教师具有对所有提交的完全访问权限。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d0542bec537b8317a46e98c215768f5228f9a07c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457647"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="56011-107">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="56011-107">Get educationSubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56011-108">检索特定的提交。</span><span class="sxs-lookup"><span data-stu-id="56011-108">Retrieve a particular submission.</span></span> <span data-ttu-id="56011-109">提交对象表示学生的工作分配。</span><span class="sxs-lookup"><span data-stu-id="56011-109">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="56011-110">与提交相关联的资源表示这一工作。</span><span class="sxs-lookup"><span data-stu-id="56011-110">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="56011-111">仅向其分配提交的学生可以查看和修改提交。</span><span class="sxs-lookup"><span data-stu-id="56011-111">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="56011-112">教师具有对所有提交的完全访问权限。</span><span class="sxs-lookup"><span data-stu-id="56011-112">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="56011-113">教师的评分和反馈也是此对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="56011-113">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="56011-114">只有教师可以添加或更改成绩和反馈。</span><span class="sxs-lookup"><span data-stu-id="56011-114">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="56011-115">在发布工作分配之前, 学生将看不到评分或反馈。</span><span class="sxs-lookup"><span data-stu-id="56011-115">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="56011-116">基本权限不包括评分和反馈, 但包括其他所有内容。</span><span class="sxs-lookup"><span data-stu-id="56011-116">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="56011-117">权限</span><span class="sxs-lookup"><span data-stu-id="56011-117">Permissions</span></span>
<span data-ttu-id="56011-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56011-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56011-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="56011-120">Permission type</span></span>      | <span data-ttu-id="56011-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56011-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56011-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56011-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="56011-123">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="56011-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="56011-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56011-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="56011-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="56011-125">Not supported.</span></span>  |
|<span data-ttu-id="56011-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="56011-126">Application</span></span> | <span data-ttu-id="56011-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="56011-127">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="56011-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56011-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56011-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="56011-129">Optional query parameters</span></span>
<span data-ttu-id="56011-130">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="56011-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56011-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="56011-131">Request headers</span></span>
| <span data-ttu-id="56011-132">标头</span><span class="sxs-lookup"><span data-stu-id="56011-132">Header</span></span>       | <span data-ttu-id="56011-133">值</span><span class="sxs-lookup"><span data-stu-id="56011-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="56011-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="56011-134">Authorization</span></span>  | <span data-ttu-id="56011-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56011-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56011-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="56011-137">Request body</span></span>
<span data-ttu-id="56011-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56011-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="56011-139">响应</span><span class="sxs-lookup"><span data-stu-id="56011-139">Response</span></span>
<span data-ttu-id="56011-140">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationSubmission](../resources/educationsubmission.md)对象。</span><span class="sxs-lookup"><span data-stu-id="56011-140">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56011-141">示例</span><span class="sxs-lookup"><span data-stu-id="56011-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56011-142">请求</span><span class="sxs-lookup"><span data-stu-id="56011-142">Request</span></span>
<span data-ttu-id="56011-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56011-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="56011-144">响应</span><span class="sxs-lookup"><span data-stu-id="56011-144">Response</span></span>
<span data-ttu-id="56011-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56011-145">The following is an example of the response.</span></span> 

><span data-ttu-id="56011-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="56011-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 712

{
    "feedback": {
      text: {
        "content": "Good work!",
        "contentType": "Text"
      },
      feedbackDateTime: "2014-01-01T00:00:00Z",
      feedbackBy: {
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
        },
        "gradedDateTime": "2014-01-01T00:00:00Z"
      },
      "id": "33223",
      "recipient": {
        "userId": "13015"
      },
      "releasedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
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
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
