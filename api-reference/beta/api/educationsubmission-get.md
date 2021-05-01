---
title: 获取 educationSubmission
description: '检索特定提交。 提交对象表示学生作业的工作。 与提交关联的资源表示此工作。 只有分配提交的学生才能查看和修改提交。 具有应用程序权限的教师或应用程序具有所有提交的完全访问权限。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 46b04c06497075d9abdb8e09533c46f752fb3e92
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2021
ms.locfileid: "52118987"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="dc328-107">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="dc328-107">Get educationSubmission</span></span>

<span data-ttu-id="dc328-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc328-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc328-109">检索特定提交。</span><span class="sxs-lookup"><span data-stu-id="dc328-109">Retrieve a particular submission.</span></span> <span data-ttu-id="dc328-110">提交对象表示学生作业的工作。</span><span class="sxs-lookup"><span data-stu-id="dc328-110">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="dc328-111">与提交关联的资源表示此工作。</span><span class="sxs-lookup"><span data-stu-id="dc328-111">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="dc328-112">只有分配提交的学生才能查看和修改提交。</span><span class="sxs-lookup"><span data-stu-id="dc328-112">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="dc328-113">具有应用程序权限的教师或应用程序具有所有提交的完全访问权限。</span><span class="sxs-lookup"><span data-stu-id="dc328-113">A teacher or application with application permissions has full access to all submissions.</span></span>

<span data-ttu-id="dc328-114">教师的成绩和反馈是与此 [对象关联的 educationOutcome](../resources/educationoutcome.md) 的一部分。</span><span class="sxs-lookup"><span data-stu-id="dc328-114">The grade and feedback from a teacher are part of the [educationOutcome](../resources/educationoutcome.md) associated with this object.</span></span> <span data-ttu-id="dc328-115">只有具有应用程序权限的教师或应用程序才能添加或更改成绩和反馈。</span><span class="sxs-lookup"><span data-stu-id="dc328-115">Only teachers or applications with application permissions can add or change grades and feedback.</span></span> <span data-ttu-id="dc328-116">在作业发布之前，学生将看不到成绩或反馈。</span><span class="sxs-lookup"><span data-stu-id="dc328-116">Students will not see the grade or feedback until the assignment has been released.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc328-117">权限</span><span class="sxs-lookup"><span data-stu-id="dc328-117">Permissions</span></span>
<span data-ttu-id="dc328-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc328-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc328-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc328-120">Permission type</span></span>      | <span data-ttu-id="dc328-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc328-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc328-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc328-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="dc328-123">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc328-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="dc328-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc328-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dc328-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc328-125">Not supported.</span></span>  |
|<span data-ttu-id="dc328-126">Application\*</span><span class="sxs-lookup"><span data-stu-id="dc328-126">Application\*</span></span> | <span data-ttu-id="dc328-127">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc328-127">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="dc328-128">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="dc328-128">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="dc328-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc328-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dc328-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dc328-130">Optional query parameters</span></span>
<span data-ttu-id="dc328-131">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dc328-131">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc328-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc328-132">Request headers</span></span>
| <span data-ttu-id="dc328-133">标头</span><span class="sxs-lookup"><span data-stu-id="dc328-133">Header</span></span>       | <span data-ttu-id="dc328-134">值</span><span class="sxs-lookup"><span data-stu-id="dc328-134">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc328-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc328-135">Authorization</span></span>  | <span data-ttu-id="dc328-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc328-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc328-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc328-138">Request body</span></span>
<span data-ttu-id="dc328-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc328-139">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dc328-140">响应</span><span class="sxs-lookup"><span data-stu-id="dc328-140">Response</span></span>
<span data-ttu-id="dc328-141">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationSubmission](../resources/educationsubmission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc328-141">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc328-142">示例</span><span class="sxs-lookup"><span data-stu-id="dc328-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc328-143">请求</span><span class="sxs-lookup"><span data-stu-id="dc328-143">Request</span></span>
<span data-ttu-id="dc328-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dc328-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc328-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc328-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
# <a name="c"></a>[<span data-ttu-id="dc328-146">C#</span><span class="sxs-lookup"><span data-stu-id="dc328-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc328-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc328-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc328-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc328-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc328-149">Java</span><span class="sxs-lookup"><span data-stu-id="dc328-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dc328-150">响应</span><span class="sxs-lookup"><span data-stu-id="dc328-150">Response</span></span>
<span data-ttu-id="dc328-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dc328-151">The following is an example of the response.</span></span> 

><span data-ttu-id="dc328-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dc328-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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
