---
title: educationAssignment：发布
description: 此操作将工作分配的状态从其原始草稿状态更改为 "已发布" 状态。 只有班级中的一名教师可以进行此呼叫。 当工作分配处于草稿状态时，学生将看不到该工作分配，也不会有任何提交对象。 调用此 API 时，将创建提交对象，并且该工作分配将显示在学生的列表中。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8bd23a420c5f4ca3b5e8a666b8b4a153e602fb34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007761"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="888cc-106">educationAssignment：发布</span><span class="sxs-lookup"><span data-stu-id="888cc-106">educationAssignment: publish</span></span>

<span data-ttu-id="888cc-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="888cc-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="888cc-108">此操作将工作分配的状态从其原始草稿状态更改为 "已发布" 状态。</span><span class="sxs-lookup"><span data-stu-id="888cc-108">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="888cc-109">只有班级中的一名教师可以进行此呼叫。</span><span class="sxs-lookup"><span data-stu-id="888cc-109">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="888cc-110">当工作分配处于草稿状态时，学生将看不到该工作分配，也不会有任何提交对象。</span><span class="sxs-lookup"><span data-stu-id="888cc-110">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="888cc-111">调用此 API 时，将创建提交对象，并且该工作分配将显示在学生的列表中。</span><span class="sxs-lookup"><span data-stu-id="888cc-111">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="888cc-112">权限</span><span class="sxs-lookup"><span data-stu-id="888cc-112">Permissions</span></span>
<span data-ttu-id="888cc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="888cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="888cc-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="888cc-115">Permission type</span></span>      | <span data-ttu-id="888cc-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="888cc-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="888cc-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="888cc-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="888cc-118">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="888cc-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="888cc-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="888cc-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="888cc-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="888cc-120">Not supported.</span></span>  |
|<span data-ttu-id="888cc-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="888cc-121">Application</span></span> | <span data-ttu-id="888cc-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="888cc-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="888cc-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="888cc-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="888cc-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="888cc-124">Request headers</span></span>
| <span data-ttu-id="888cc-125">标头</span><span class="sxs-lookup"><span data-stu-id="888cc-125">Header</span></span>       | <span data-ttu-id="888cc-126">值</span><span class="sxs-lookup"><span data-stu-id="888cc-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="888cc-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="888cc-127">Authorization</span></span>  | <span data-ttu-id="888cc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="888cc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="888cc-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="888cc-130">Request body</span></span>
<span data-ttu-id="888cc-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="888cc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="888cc-132">响应</span><span class="sxs-lookup"><span data-stu-id="888cc-132">Response</span></span>
<span data-ttu-id="888cc-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="888cc-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="888cc-135">示例</span><span class="sxs-lookup"><span data-stu-id="888cc-135">Example</span></span>
<span data-ttu-id="888cc-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="888cc-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="888cc-137">请求</span><span class="sxs-lookup"><span data-stu-id="888cc-137">Request</span></span>
<span data-ttu-id="888cc-138">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="888cc-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="888cc-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="888cc-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```
# <a name="c"></a>[<span data-ttu-id="888cc-140">C#</span><span class="sxs-lookup"><span data-stu-id="888cc-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="888cc-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="888cc-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="888cc-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="888cc-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="888cc-143">响应</span><span class="sxs-lookup"><span data-stu-id="888cc-143">Response</span></span>
<span data-ttu-id="888cc-144">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="888cc-144">The following is an example of a response.</span></span> 

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
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


