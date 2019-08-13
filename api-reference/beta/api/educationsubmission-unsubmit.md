---
title: 'educationSubmission: unsubmit'
description: '一个操作, 指示学生希望在工作分配在打开后进行提交。 仅学生可以执行此操作。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 702d0d1e5dc18838c87ffa37ab5628e0f924e378
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323804"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="f06e3-104">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="f06e3-104">educationSubmission: unsubmit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f06e3-105">一个操作, 指示学生希望在工作分配在打开后进行提交。</span><span class="sxs-lookup"><span data-stu-id="f06e3-105">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="f06e3-106">仅学生可以执行此操作。</span><span class="sxs-lookup"><span data-stu-id="f06e3-106">This action can only be taken by the student.</span></span> <span data-ttu-id="f06e3-107">这会将提交的状态从 "已提交" 更改为 "正在运行"。</span><span class="sxs-lookup"><span data-stu-id="f06e3-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="f06e3-108">在提交过程中, 所有资源都将从 submittedResources 复制到 workingResources 存储桶。</span><span class="sxs-lookup"><span data-stu-id="f06e3-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="f06e3-109">教师将查看用于评分的工作资源列表。</span><span class="sxs-lookup"><span data-stu-id="f06e3-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="f06e3-110">权限</span><span class="sxs-lookup"><span data-stu-id="f06e3-110">Permissions</span></span>
<span data-ttu-id="f06e3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f06e3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f06e3-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f06e3-113">Permission type</span></span>      | <span data-ttu-id="f06e3-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f06e3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f06e3-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f06e3-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="f06e3-116">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="f06e3-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f06e3-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f06e3-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f06e3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f06e3-118">Not supported.</span></span>  |
|<span data-ttu-id="f06e3-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="f06e3-119">Application</span></span> | <span data-ttu-id="f06e3-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="f06e3-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f06e3-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f06e3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="f06e3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f06e3-122">Request headers</span></span>
| <span data-ttu-id="f06e3-123">标头</span><span class="sxs-lookup"><span data-stu-id="f06e3-123">Header</span></span>       | <span data-ttu-id="f06e3-124">值</span><span class="sxs-lookup"><span data-stu-id="f06e3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f06e3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f06e3-125">Authorization</span></span>  | <span data-ttu-id="f06e3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f06e3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f06e3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f06e3-128">Request body</span></span>
<span data-ttu-id="f06e3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f06e3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f06e3-130">响应</span><span class="sxs-lookup"><span data-stu-id="f06e3-130">Response</span></span>
<span data-ttu-id="f06e3-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f06e3-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f06e3-133">示例</span><span class="sxs-lookup"><span data-stu-id="f06e3-133">Example</span></span>
<span data-ttu-id="f06e3-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f06e3-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f06e3-135">请求</span><span class="sxs-lookup"><span data-stu-id="f06e3-135">Request</span></span>
<span data-ttu-id="f06e3-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f06e3-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f06e3-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f06e3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f06e3-138">C#</span><span class="sxs-lookup"><span data-stu-id="f06e3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f06e3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f06e3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f06e3-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="f06e3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f06e3-141">Java</span><span class="sxs-lookup"><span data-stu-id="f06e3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-unsubmit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f06e3-142">响应</span><span class="sxs-lookup"><span data-stu-id="f06e3-142">Response</span></span>
<span data-ttu-id="f06e3-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f06e3-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
