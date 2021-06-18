---
title: educationSubmission：未提交
description: 指示学生想要在作业提交后处理作业提交。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4ddad6241c4e6c7820db143e93064b4570d68e49
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993270"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="63534-103">educationSubmission：未提交</span><span class="sxs-lookup"><span data-stu-id="63534-103">educationSubmission: unsubmit</span></span>

<span data-ttu-id="63534-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63534-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63534-105">指示学生想要在作业提交后处理作业提交。</span><span class="sxs-lookup"><span data-stu-id="63534-105">Indicate that a student wants to work on the submission of the assignment after it was turned in.</span></span> 

<span data-ttu-id="63534-106">此操作仅能由学生执行。</span><span class="sxs-lookup"><span data-stu-id="63534-106">This action can only be taken by the student.</span></span> <span data-ttu-id="63534-107">这会将提交状态从"已提交"更改为"正在工作"。</span><span class="sxs-lookup"><span data-stu-id="63534-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="63534-108">在提交过程中，所有资源都将从 submittedResources 复制到 workingResources 存储桶。</span><span class="sxs-lookup"><span data-stu-id="63534-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="63534-109">教师将查看工作资源列表进行评分。</span><span class="sxs-lookup"><span data-stu-id="63534-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="63534-110">权限</span><span class="sxs-lookup"><span data-stu-id="63534-110">Permissions</span></span>
<span data-ttu-id="63534-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63534-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63534-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="63534-113">Permission type</span></span>      | <span data-ttu-id="63534-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63534-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63534-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63534-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="63534-116">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63534-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="63534-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63534-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="63534-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="63534-118">Not supported.</span></span>  |
|<span data-ttu-id="63534-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="63534-119">Application</span></span> | <span data-ttu-id="63534-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="63534-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="63534-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63534-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="63534-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="63534-122">Request headers</span></span>
| <span data-ttu-id="63534-123">标头</span><span class="sxs-lookup"><span data-stu-id="63534-123">Header</span></span>       | <span data-ttu-id="63534-124">值</span><span class="sxs-lookup"><span data-stu-id="63534-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63534-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="63534-125">Authorization</span></span>  | <span data-ttu-id="63534-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63534-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63534-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="63534-128">Request body</span></span>
<span data-ttu-id="63534-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63534-129">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63534-130">响应</span><span class="sxs-lookup"><span data-stu-id="63534-130">Response</span></span>
<span data-ttu-id="63534-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="63534-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63534-133">示例</span><span class="sxs-lookup"><span data-stu-id="63534-133">Example</span></span>
<span data-ttu-id="63534-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="63534-134">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="63534-135">请求</span><span class="sxs-lookup"><span data-stu-id="63534-135">Request</span></span>
<span data-ttu-id="63534-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63534-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="63534-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="63534-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/unsubmit
```
# <a name="c"></a>[<span data-ttu-id="63534-138">C#</span><span class="sxs-lookup"><span data-stu-id="63534-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63534-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63534-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63534-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63534-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63534-141">Java</span><span class="sxs-lookup"><span data-stu-id="63534-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-unsubmit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63534-142">响应</span><span class="sxs-lookup"><span data-stu-id="63534-142">Response</span></span>
<span data-ttu-id="63534-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63534-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content

{
}
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


