---
title: educationAssignment： publish
description: 此操作将工作分配的状态从原始草稿状态更改为已发布状态。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3badfbf152188a0a999c41f1bcb2edffce3bf9f9
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911919"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="dd2e1-103">educationAssignment： publish</span><span class="sxs-lookup"><span data-stu-id="dd2e1-103">educationAssignment: publish</span></span>

<span data-ttu-id="dd2e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd2e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd2e1-105">此操作将工作分配的状态从原始草稿状态更改为已发布状态。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-105">This action changes the state of an assignment from its original draft status to the published status.</span></span> 

<span data-ttu-id="dd2e1-106">只有课堂中的教师才能进行此呼叫。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-106">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="dd2e1-107">当作业在草稿状态时，学生将看不到作业，也不会看到任何提交对象。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-107">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="dd2e1-108">调用此 API 时，将创建提交对象，作业将显示在学生列表中。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-108">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd2e1-109">权限</span><span class="sxs-lookup"><span data-stu-id="dd2e1-109">Permissions</span></span>
<span data-ttu-id="dd2e1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd2e1-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd2e1-112">Permission type</span></span>      | <span data-ttu-id="dd2e1-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd2e1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd2e1-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd2e1-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="dd2e1-115">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd2e1-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="dd2e1-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd2e1-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dd2e1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-117">Not supported.</span></span>  |
|<span data-ttu-id="dd2e1-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd2e1-118">Application</span></span> | <span data-ttu-id="dd2e1-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dd2e1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd2e1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="dd2e1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd2e1-121">Request headers</span></span>
| <span data-ttu-id="dd2e1-122">标头</span><span class="sxs-lookup"><span data-stu-id="dd2e1-122">Header</span></span>       | <span data-ttu-id="dd2e1-123">值</span><span class="sxs-lookup"><span data-stu-id="dd2e1-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dd2e1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd2e1-124">Authorization</span></span>  | <span data-ttu-id="dd2e1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dd2e1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd2e1-127">Request body</span></span>
<span data-ttu-id="dd2e1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd2e1-129">响应</span><span class="sxs-lookup"><span data-stu-id="dd2e1-129">Response</span></span>
<span data-ttu-id="dd2e1-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd2e1-132">示例</span><span class="sxs-lookup"><span data-stu-id="dd2e1-132">Example</span></span>
<span data-ttu-id="dd2e1-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dd2e1-134">请求</span><span class="sxs-lookup"><span data-stu-id="dd2e1-134">Request</span></span>
<span data-ttu-id="dd2e1-135">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd2e1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd2e1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish_2"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```
# <a name="c"></a>[<span data-ttu-id="dd2e1-137">C#</span><span class="sxs-lookup"><span data-stu-id="dd2e1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd2e1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd2e1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd2e1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd2e1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd2e1-140">Java</span><span class="sxs-lookup"><span data-stu-id="dd2e1-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd2e1-141">响应</span><span class="sxs-lookup"><span data-stu-id="dd2e1-141">Response</span></span>
<span data-ttu-id="dd2e1-142">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="dd2e1-142">The following is an example of a response.</span></span> 

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


