---
title: 删除 educationAssignmentResource
description: 删除附加到工作分配的特定资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7e853534998978f89e44cbd8f657a56250c599a0
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911903"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="211fc-103">删除 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="211fc-103">Delete educationAssignmentResource</span></span>

<span data-ttu-id="211fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="211fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="211fc-105">删除附加到工作分配的特定资源。</span><span class="sxs-lookup"><span data-stu-id="211fc-105">Delete a specific resource attached to an assignment.</span></span> <span data-ttu-id="211fc-106">只有班级中的教师可以删除资源。</span><span class="sxs-lookup"><span data-stu-id="211fc-106">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="211fc-107">向学生发布作业后，教师无法删除标记为"distributeToStudents"的资源。</span><span class="sxs-lookup"><span data-stu-id="211fc-107">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="211fc-108">权限</span><span class="sxs-lookup"><span data-stu-id="211fc-108">Permissions</span></span>
<span data-ttu-id="211fc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="211fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="211fc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="211fc-111">Permission type</span></span>      | <span data-ttu-id="211fc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="211fc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="211fc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="211fc-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="211fc-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="211fc-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="211fc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="211fc-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="211fc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="211fc-116">Not supported.</span></span>  |
|<span data-ttu-id="211fc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="211fc-117">Application</span></span> | <span data-ttu-id="211fc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="211fc-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="211fc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="211fc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="211fc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="211fc-120">Request headers</span></span>
| <span data-ttu-id="211fc-121">标头</span><span class="sxs-lookup"><span data-stu-id="211fc-121">Header</span></span>       | <span data-ttu-id="211fc-122">值</span><span class="sxs-lookup"><span data-stu-id="211fc-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="211fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="211fc-123">Authorization</span></span>  | <span data-ttu-id="211fc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="211fc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="211fc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="211fc-126">Request body</span></span>
<span data-ttu-id="211fc-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="211fc-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="211fc-128">响应</span><span class="sxs-lookup"><span data-stu-id="211fc-128">Response</span></span>
<span data-ttu-id="211fc-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="211fc-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="211fc-131">示例</span><span class="sxs-lookup"><span data-stu-id="211fc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="211fc-132">请求</span><span class="sxs-lookup"><span data-stu-id="211fc-132">Request</span></span>
<span data-ttu-id="211fc-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="211fc-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="211fc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="211fc-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="211fc-135">C#</span><span class="sxs-lookup"><span data-stu-id="211fc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="211fc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="211fc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="211fc-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="211fc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="211fc-138">Java</span><span class="sxs-lookup"><span data-stu-id="211fc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="211fc-139">响应</span><span class="sxs-lookup"><span data-stu-id="211fc-139">Response</span></span>
<span data-ttu-id="211fc-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="211fc-140">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


