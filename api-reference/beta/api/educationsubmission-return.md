---
title: educationSubmission： return
description: 此操作可使学生获得与此提交相关的成绩和反馈。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: da0f7f6c92ce5c0782f076ad10280355e4a009c0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787287"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="1585c-103">educationSubmission： return</span><span class="sxs-lookup"><span data-stu-id="1585c-103">educationSubmission: return</span></span>

<span data-ttu-id="1585c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1585c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1585c-105">此操作可使学生获得与此提交相关的成绩和反馈。</span><span class="sxs-lookup"><span data-stu-id="1585c-105">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="1585c-106">这会将提交状态从"已提交"更改为"已返回"，并指示提供了反馈或评分已完成。</span><span class="sxs-lookup"><span data-stu-id="1585c-106">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="1585c-107">此操作仅能由教师执行。</span><span class="sxs-lookup"><span data-stu-id="1585c-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="1585c-108">权限</span><span class="sxs-lookup"><span data-stu-id="1585c-108">Permissions</span></span>
<span data-ttu-id="1585c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1585c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1585c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1585c-111">Permission type</span></span>      | <span data-ttu-id="1585c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1585c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1585c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1585c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="1585c-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1585c-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="1585c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1585c-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1585c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1585c-116">Not supported.</span></span>  |
|<span data-ttu-id="1585c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1585c-117">Application</span></span> | <span data-ttu-id="1585c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1585c-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1585c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1585c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return
```
## <a name="request-headers"></a><span data-ttu-id="1585c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1585c-120">Request headers</span></span>
| <span data-ttu-id="1585c-121">标头</span><span class="sxs-lookup"><span data-stu-id="1585c-121">Header</span></span>       | <span data-ttu-id="1585c-122">值</span><span class="sxs-lookup"><span data-stu-id="1585c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1585c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1585c-123">Authorization</span></span>  | <span data-ttu-id="1585c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1585c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1585c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1585c-126">Request body</span></span>
<span data-ttu-id="1585c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1585c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1585c-128">响应</span><span class="sxs-lookup"><span data-stu-id="1585c-128">Response</span></span>
<span data-ttu-id="1585c-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1585c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1585c-131">示例</span><span class="sxs-lookup"><span data-stu-id="1585c-131">Example</span></span>
<span data-ttu-id="1585c-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1585c-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1585c-133">请求</span><span class="sxs-lookup"><span data-stu-id="1585c-133">Request</span></span>
<span data-ttu-id="1585c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1585c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1585c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1585c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```
# <a name="c"></a>[<span data-ttu-id="1585c-136">C#</span><span class="sxs-lookup"><span data-stu-id="1585c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-return-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1585c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1585c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-return-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1585c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1585c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-return-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1585c-139">Java</span><span class="sxs-lookup"><span data-stu-id="1585c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-return-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1585c-140">响应</span><span class="sxs-lookup"><span data-stu-id="1585c-140">Response</span></span>
<span data-ttu-id="1585c-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1585c-141">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


