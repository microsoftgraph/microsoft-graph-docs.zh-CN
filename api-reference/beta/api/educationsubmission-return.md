---
title: educationSubmission：返回
description: 此操作使与此提交相关联的评分和反馈可供学生使用。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d04c954f239ba1999f2ca838d14e52b7920f4bc0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424825"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="08100-103">educationSubmission：返回</span><span class="sxs-lookup"><span data-stu-id="08100-103">educationSubmission: return</span></span>

<span data-ttu-id="08100-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="08100-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08100-105">此操作使与此提交相关联的评分和反馈可供学生使用。</span><span class="sxs-lookup"><span data-stu-id="08100-105">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="08100-106">这会将提交的状态从 "已提交" 更改为 "已返回"，并指示反馈已提供或已完成评分。</span><span class="sxs-lookup"><span data-stu-id="08100-106">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="08100-107">此操作仅可由教师完成。</span><span class="sxs-lookup"><span data-stu-id="08100-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="08100-108">权限</span><span class="sxs-lookup"><span data-stu-id="08100-108">Permissions</span></span>
<span data-ttu-id="08100-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08100-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08100-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="08100-111">Permission type</span></span>      | <span data-ttu-id="08100-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08100-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08100-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08100-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="08100-114">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="08100-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="08100-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08100-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="08100-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="08100-116">Not supported.</span></span>  |
|<span data-ttu-id="08100-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="08100-117">Application</span></span> | <span data-ttu-id="08100-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="08100-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="08100-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08100-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="08100-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="08100-120">Request headers</span></span>
| <span data-ttu-id="08100-121">标头</span><span class="sxs-lookup"><span data-stu-id="08100-121">Header</span></span>       | <span data-ttu-id="08100-122">值</span><span class="sxs-lookup"><span data-stu-id="08100-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08100-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08100-123">Authorization</span></span>  | <span data-ttu-id="08100-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08100-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08100-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="08100-126">Request body</span></span>
<span data-ttu-id="08100-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="08100-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08100-128">响应</span><span class="sxs-lookup"><span data-stu-id="08100-128">Response</span></span>
<span data-ttu-id="08100-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="08100-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08100-131">示例</span><span class="sxs-lookup"><span data-stu-id="08100-131">Example</span></span>
<span data-ttu-id="08100-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="08100-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="08100-133">请求</span><span class="sxs-lookup"><span data-stu-id="08100-133">Request</span></span>
<span data-ttu-id="08100-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08100-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08100-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="08100-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```
# <a name="c"></a>[<span data-ttu-id="08100-136">C#</span><span class="sxs-lookup"><span data-stu-id="08100-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-return-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08100-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08100-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-return-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08100-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08100-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-return-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08100-139">响应</span><span class="sxs-lookup"><span data-stu-id="08100-139">Response</span></span>
<span data-ttu-id="08100-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="08100-140">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
