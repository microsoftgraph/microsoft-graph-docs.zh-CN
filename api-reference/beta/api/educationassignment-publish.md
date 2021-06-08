---
title: educationAssignment： publish
description: 此操作将工作分配的状态从原始草稿状态更改为已发布状态。 只有课堂中的教师才能进行此呼叫。 当作业在草稿状态时，学生将看不到作业，也不会看到任何提交对象。 调用此 API 时，将创建提交对象，作业将显示在学生列表中。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ac840109209b2a8ec5081d55abc31e1fac92d965
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785996"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="d25b6-106">educationAssignment： publish</span><span class="sxs-lookup"><span data-stu-id="d25b6-106">educationAssignment: publish</span></span>

<span data-ttu-id="d25b6-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d25b6-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d25b6-108">此操作将工作分配的状态从原始草稿状态更改为已发布状态。</span><span class="sxs-lookup"><span data-stu-id="d25b6-108">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="d25b6-109">只有课堂中的教师才能进行此呼叫。</span><span class="sxs-lookup"><span data-stu-id="d25b6-109">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="d25b6-110">当作业在草稿状态时，学生将看不到作业，也不会看到任何提交对象。</span><span class="sxs-lookup"><span data-stu-id="d25b6-110">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="d25b6-111">调用此 API 时，将创建提交对象，作业将显示在学生列表中。</span><span class="sxs-lookup"><span data-stu-id="d25b6-111">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="d25b6-112">权限</span><span class="sxs-lookup"><span data-stu-id="d25b6-112">Permissions</span></span>
<span data-ttu-id="d25b6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d25b6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d25b6-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="d25b6-115">Permission type</span></span>      | <span data-ttu-id="d25b6-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d25b6-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d25b6-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d25b6-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="d25b6-118">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d25b6-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d25b6-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d25b6-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d25b6-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="d25b6-120">Not supported.</span></span>  |
|<span data-ttu-id="d25b6-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="d25b6-121">Application</span></span> | <span data-ttu-id="d25b6-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="d25b6-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d25b6-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d25b6-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="d25b6-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="d25b6-124">Request headers</span></span>
| <span data-ttu-id="d25b6-125">标头</span><span class="sxs-lookup"><span data-stu-id="d25b6-125">Header</span></span>       | <span data-ttu-id="d25b6-126">值</span><span class="sxs-lookup"><span data-stu-id="d25b6-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d25b6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d25b6-127">Authorization</span></span>  | <span data-ttu-id="d25b6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d25b6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d25b6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d25b6-130">Request body</span></span>
<span data-ttu-id="d25b6-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d25b6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d25b6-132">响应</span><span class="sxs-lookup"><span data-stu-id="d25b6-132">Response</span></span>
<span data-ttu-id="d25b6-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d25b6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d25b6-135">示例</span><span class="sxs-lookup"><span data-stu-id="d25b6-135">Example</span></span>
<span data-ttu-id="d25b6-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d25b6-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d25b6-137">请求</span><span class="sxs-lookup"><span data-stu-id="d25b6-137">Request</span></span>
<span data-ttu-id="d25b6-138">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="d25b6-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d25b6-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d25b6-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish_2"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```
# <a name="c"></a>[<span data-ttu-id="d25b6-140">C#</span><span class="sxs-lookup"><span data-stu-id="d25b6-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d25b6-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d25b6-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d25b6-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d25b6-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d25b6-143">Java</span><span class="sxs-lookup"><span data-stu-id="d25b6-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d25b6-144">响应</span><span class="sxs-lookup"><span data-stu-id="d25b6-144">Response</span></span>
<span data-ttu-id="d25b6-145">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="d25b6-145">The following is an example of a response.</span></span> 

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
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


