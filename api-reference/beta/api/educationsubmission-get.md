---
title: 获取 educationSubmission
description: '检索特定提交。 一个提交对象，代表学生的工作分配。 提交表示与此工作关联资源。 仅提交分配给学生可以查看和修改提交。 教师具有所有提交到的完全访问权限。 '
ms.openlocfilehash: 016e8d2e04377ec24fa55ad940fb97364786f433
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045262"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="fa141-107">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="fa141-107">Get educationSubmission</span></span>

> <span data-ttu-id="fa141-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fa141-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa141-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fa141-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa141-110">检索特定提交。</span><span class="sxs-lookup"><span data-stu-id="fa141-110">Retrieve a particular submission.</span></span> <span data-ttu-id="fa141-111">一个提交对象，代表学生的工作分配。</span><span class="sxs-lookup"><span data-stu-id="fa141-111">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="fa141-112">提交表示与此工作关联资源。</span><span class="sxs-lookup"><span data-stu-id="fa141-112">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="fa141-113">仅提交分配给学生可以查看和修改提交。</span><span class="sxs-lookup"><span data-stu-id="fa141-113">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="fa141-114">教师具有所有提交到的完全访问权限。</span><span class="sxs-lookup"><span data-stu-id="fa141-114">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="fa141-115">薪等级和教师的反馈也是此对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="fa141-115">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="fa141-116">仅教师可以添加或更改薪等级和反馈。</span><span class="sxs-lookup"><span data-stu-id="fa141-116">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="fa141-117">已发布工作分配之前，学生将不会看到薪等级或反馈。</span><span class="sxs-lookup"><span data-stu-id="fa141-117">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="fa141-118">基本权限不包括薪等级和反馈，但包含其他所有内容。</span><span class="sxs-lookup"><span data-stu-id="fa141-118">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa141-119">权限</span><span class="sxs-lookup"><span data-stu-id="fa141-119">Permissions</span></span>
<span data-ttu-id="fa141-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa141-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa141-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa141-122">Permission type</span></span>      | <span data-ttu-id="fa141-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa141-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa141-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa141-124">Delegated (work or school account)</span></span> |  <span data-ttu-id="fa141-125">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa141-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="fa141-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa141-126">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fa141-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa141-127">Not supported.</span></span>  |
|<span data-ttu-id="fa141-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa141-128">Application</span></span> | <span data-ttu-id="fa141-129">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa141-129">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fa141-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa141-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa141-131">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fa141-131">Optional query parameters</span></span>
<span data-ttu-id="fa141-132">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fa141-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa141-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa141-133">Request headers</span></span>
| <span data-ttu-id="fa141-134">标头</span><span class="sxs-lookup"><span data-stu-id="fa141-134">Header</span></span>       | <span data-ttu-id="fa141-135">值</span><span class="sxs-lookup"><span data-stu-id="fa141-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa141-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa141-136">Authorization</span></span>  | <span data-ttu-id="fa141-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa141-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa141-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa141-139">Request body</span></span>
<span data-ttu-id="fa141-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa141-140">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fa141-141">响应</span><span class="sxs-lookup"><span data-stu-id="fa141-141">Response</span></span>
<span data-ttu-id="fa141-142">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationSubmission](../resources/educationsubmission.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fa141-142">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa141-143">示例</span><span class="sxs-lookup"><span data-stu-id="fa141-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa141-144">请求</span><span class="sxs-lookup"><span data-stu-id="fa141-144">Request</span></span>
<span data-ttu-id="fa141-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fa141-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="fa141-146">响应</span><span class="sxs-lookup"><span data-stu-id="fa141-146">Response</span></span>
<span data-ttu-id="fa141-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fa141-147">The following is an example of the response.</span></span> 

><span data-ttu-id="fa141-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fa141-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->