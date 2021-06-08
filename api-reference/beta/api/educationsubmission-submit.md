---
title: educationSubmission： submit
description: 指示学生已完成工作并准备好处理作业的操作。 此操作仅能由学生执行。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2f33bea764c76ccc3a320bd610249cedf372071f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787280"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="93a6b-104">educationSubmission： submit</span><span class="sxs-lookup"><span data-stu-id="93a6b-104">educationSubmission: submit</span></span>

<span data-ttu-id="93a6b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93a6b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93a6b-106">指示学生已完成工作并准备好处理作业的操作。</span><span class="sxs-lookup"><span data-stu-id="93a6b-106">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="93a6b-107">此操作仅能由学生执行。</span><span class="sxs-lookup"><span data-stu-id="93a6b-107">This action can only be taken by the student.</span></span> <span data-ttu-id="93a6b-108">这会将提交状态从"正在工作"更改为"已提交"。</span><span class="sxs-lookup"><span data-stu-id="93a6b-108">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="93a6b-109">在提交过程中，所有资源都将复制到 **submittedResources** 存储桶。</span><span class="sxs-lookup"><span data-stu-id="93a6b-109">During the submit process, all the resources will be copied to the **submittedResources** bucket.</span></span> <span data-ttu-id="93a6b-110">教师将查看提交的资源列表进行评分。</span><span class="sxs-lookup"><span data-stu-id="93a6b-110">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="93a6b-111">权限</span><span class="sxs-lookup"><span data-stu-id="93a6b-111">Permissions</span></span>
<span data-ttu-id="93a6b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93a6b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93a6b-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="93a6b-114">Permission type</span></span>      | <span data-ttu-id="93a6b-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93a6b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93a6b-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93a6b-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="93a6b-117">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93a6b-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="93a6b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93a6b-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="93a6b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="93a6b-119">Not supported.</span></span>  |
|<span data-ttu-id="93a6b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="93a6b-120">Application</span></span> | <span data-ttu-id="93a6b-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="93a6b-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="93a6b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93a6b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit
```

## <a name="request-headers"></a><span data-ttu-id="93a6b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="93a6b-123">Request headers</span></span>
| <span data-ttu-id="93a6b-124">标头</span><span class="sxs-lookup"><span data-stu-id="93a6b-124">Header</span></span>       | <span data-ttu-id="93a6b-125">值</span><span class="sxs-lookup"><span data-stu-id="93a6b-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93a6b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="93a6b-126">Authorization</span></span>  | <span data-ttu-id="93a6b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93a6b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93a6b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="93a6b-129">Request body</span></span>
<span data-ttu-id="93a6b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="93a6b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93a6b-131">响应</span><span class="sxs-lookup"><span data-stu-id="93a6b-131">Response</span></span>
<span data-ttu-id="93a6b-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="93a6b-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93a6b-134">示例</span><span class="sxs-lookup"><span data-stu-id="93a6b-134">Example</span></span>
<span data-ttu-id="93a6b-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="93a6b-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="93a6b-136">请求</span><span class="sxs-lookup"><span data-stu-id="93a6b-136">Request</span></span>
<span data-ttu-id="93a6b-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="93a6b-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93a6b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="93a6b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```
# <a name="c"></a>[<span data-ttu-id="93a6b-139">C#</span><span class="sxs-lookup"><span data-stu-id="93a6b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-submit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93a6b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93a6b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-submit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93a6b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93a6b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-submit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93a6b-142">Java</span><span class="sxs-lookup"><span data-stu-id="93a6b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-submit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="93a6b-143">响应</span><span class="sxs-lookup"><span data-stu-id="93a6b-143">Response</span></span>
<span data-ttu-id="93a6b-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="93a6b-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


