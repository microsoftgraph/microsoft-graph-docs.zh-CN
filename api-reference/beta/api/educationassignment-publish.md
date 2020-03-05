---
title: educationAssignment：发布
description: 此操作将工作分配的状态从其原始草稿状态更改为 "已发布" 状态。 只有班级中的一名教师可以进行此呼叫。 当工作分配处于草稿状态时，学生将看不到该工作分配，也不会有任何提交对象。 调用此 API 时，将创建提交对象，并且该工作分配将显示在学生的列表中。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b5421840ada4484a0dda12bd4f7bb5959bcebbcb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427359"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="70d49-106">educationAssignment：发布</span><span class="sxs-lookup"><span data-stu-id="70d49-106">educationAssignment: publish</span></span>

<span data-ttu-id="70d49-107">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="70d49-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70d49-108">此操作将工作分配的状态从其原始草稿状态更改为 "已发布" 状态。</span><span class="sxs-lookup"><span data-stu-id="70d49-108">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="70d49-109">只有班级中的一名教师可以进行此呼叫。</span><span class="sxs-lookup"><span data-stu-id="70d49-109">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="70d49-110">当工作分配处于草稿状态时，学生将看不到该工作分配，也不会有任何提交对象。</span><span class="sxs-lookup"><span data-stu-id="70d49-110">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="70d49-111">调用此 API 时，将创建提交对象，并且该工作分配将显示在学生的列表中。</span><span class="sxs-lookup"><span data-stu-id="70d49-111">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="70d49-112">权限</span><span class="sxs-lookup"><span data-stu-id="70d49-112">Permissions</span></span>
<span data-ttu-id="70d49-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70d49-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70d49-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="70d49-115">Permission type</span></span>      | <span data-ttu-id="70d49-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70d49-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70d49-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70d49-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="70d49-118">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="70d49-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="70d49-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70d49-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="70d49-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="70d49-120">Not supported.</span></span>  |
|<span data-ttu-id="70d49-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="70d49-121">Application</span></span> | <span data-ttu-id="70d49-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="70d49-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="70d49-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70d49-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="70d49-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="70d49-124">Request headers</span></span>
| <span data-ttu-id="70d49-125">标头</span><span class="sxs-lookup"><span data-stu-id="70d49-125">Header</span></span>       | <span data-ttu-id="70d49-126">值</span><span class="sxs-lookup"><span data-stu-id="70d49-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70d49-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="70d49-127">Authorization</span></span>  | <span data-ttu-id="70d49-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70d49-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70d49-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="70d49-130">Request body</span></span>
<span data-ttu-id="70d49-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="70d49-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70d49-132">响应</span><span class="sxs-lookup"><span data-stu-id="70d49-132">Response</span></span>
<span data-ttu-id="70d49-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="70d49-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70d49-135">示例</span><span class="sxs-lookup"><span data-stu-id="70d49-135">Example</span></span>
<span data-ttu-id="70d49-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="70d49-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="70d49-137">请求</span><span class="sxs-lookup"><span data-stu-id="70d49-137">Request</span></span>
<span data-ttu-id="70d49-138">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="70d49-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70d49-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="70d49-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```
# <a name="c"></a>[<span data-ttu-id="70d49-140">C#</span><span class="sxs-lookup"><span data-stu-id="70d49-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70d49-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70d49-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70d49-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70d49-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="70d49-143">响应</span><span class="sxs-lookup"><span data-stu-id="70d49-143">Response</span></span>
<span data-ttu-id="70d49-144">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="70d49-144">The following is an example of a response.</span></span> 

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
