---
title: 获取 educationSubmission
description: '检索特定提交。 提交对象表示学生作业的工作。 与提交关联的资源表示此工作。 只有分配有提交的学生才能查看和修改提交。 教师可以完全访问所有提交。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2cc1e81608ead0c8d8adaac873dd962f369e186c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472998"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="1c953-107">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="1c953-107">Get educationSubmission</span></span>

<span data-ttu-id="1c953-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c953-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c953-109">检索特定提交。</span><span class="sxs-lookup"><span data-stu-id="1c953-109">Retrieve a particular submission.</span></span> <span data-ttu-id="1c953-110">提交对象表示学生作业的工作。</span><span class="sxs-lookup"><span data-stu-id="1c953-110">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="1c953-111">与提交关联的资源表示此工作。</span><span class="sxs-lookup"><span data-stu-id="1c953-111">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="1c953-112">只有分配有提交的学生才能查看和修改提交。</span><span class="sxs-lookup"><span data-stu-id="1c953-112">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="1c953-113">教师可以完全访问所有提交。</span><span class="sxs-lookup"><span data-stu-id="1c953-113">A teacher has full access to all submissions.</span></span>

<span data-ttu-id="1c953-114">教师的成绩和反馈是与此对象关联的 [educationOutcome](../resources/educationoutcome.md) 的一部分。</span><span class="sxs-lookup"><span data-stu-id="1c953-114">The grade and feedback from a teacher are part of the [educationOutcome](../resources/educationoutcome.md) associated with this object.</span></span> <span data-ttu-id="1c953-115">只有教师才能添加或更改成绩和反馈。</span><span class="sxs-lookup"><span data-stu-id="1c953-115">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="1c953-116">在作业发布之前，学生不会看到成绩或反馈。</span><span class="sxs-lookup"><span data-stu-id="1c953-116">Students will not see the grade or feedback until the assignment has been released.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c953-117">权限</span><span class="sxs-lookup"><span data-stu-id="1c953-117">Permissions</span></span>
<span data-ttu-id="1c953-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c953-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c953-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c953-120">Permission type</span></span>      | <span data-ttu-id="1c953-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c953-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c953-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c953-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="1c953-123">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c953-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="1c953-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c953-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1c953-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c953-125">Not supported.</span></span>  |
|<span data-ttu-id="1c953-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c953-126">Application</span></span> | <span data-ttu-id="1c953-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c953-127">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1c953-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c953-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c953-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1c953-129">Optional query parameters</span></span>
<span data-ttu-id="1c953-130">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1c953-130">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c953-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c953-131">Request headers</span></span>
| <span data-ttu-id="1c953-132">标头</span><span class="sxs-lookup"><span data-stu-id="1c953-132">Header</span></span>       | <span data-ttu-id="1c953-133">值</span><span class="sxs-lookup"><span data-stu-id="1c953-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c953-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c953-134">Authorization</span></span>  | <span data-ttu-id="1c953-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c953-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c953-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c953-137">Request body</span></span>
<span data-ttu-id="1c953-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1c953-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1c953-139">响应</span><span class="sxs-lookup"><span data-stu-id="1c953-139">Response</span></span>
<span data-ttu-id="1c953-140">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [educationSubmission](../resources/educationsubmission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c953-140">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c953-141">示例</span><span class="sxs-lookup"><span data-stu-id="1c953-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c953-142">请求</span><span class="sxs-lookup"><span data-stu-id="1c953-142">Request</span></span>
<span data-ttu-id="1c953-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1c953-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c953-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c953-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
# <a name="c"></a>[<span data-ttu-id="1c953-145">C#</span><span class="sxs-lookup"><span data-stu-id="1c953-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c953-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c953-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c953-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c953-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c953-148">Java</span><span class="sxs-lookup"><span data-stu-id="1c953-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c953-149">响应</span><span class="sxs-lookup"><span data-stu-id="1c953-149">Response</span></span>
<span data-ttu-id="1c953-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1c953-150">The following is an example of the response.</span></span> 

><span data-ttu-id="1c953-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1c953-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 712

{
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
  "suppressions": []
}
-->
