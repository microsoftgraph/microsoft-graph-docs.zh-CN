---
title: 发布教育作业
description: 此操作将发布教育作业。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0ef7011e283e9c9c1139516a0261b52e4cfdfff5
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993213"
---
# <a name="publish-an-education-assignment"></a><span data-ttu-id="383ce-103">发布教育作业</span><span class="sxs-lookup"><span data-stu-id="383ce-103">Publish an education assignment</span></span>

<span data-ttu-id="383ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="383ce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="383ce-105">此操作将发布教育作业。</span><span class="sxs-lookup"><span data-stu-id="383ce-105">This action publishes an education assignment.</span></span>

 <span data-ttu-id="383ce-106">只有课堂中的教师才能进行此呼叫。</span><span class="sxs-lookup"><span data-stu-id="383ce-106">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="383ce-107">当作业在草稿状态时，学生将看不到作业，也不会看到任何提交对象。</span><span class="sxs-lookup"><span data-stu-id="383ce-107">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="383ce-108">调用此 API 将 [创建 educationSubmission](../resources/educationsubmission.md) 对象，并在每个学生列表中显示作业。</span><span class="sxs-lookup"><span data-stu-id="383ce-108">Calling this API creates [educationSubmission](../resources/educationsubmission.md) objects and displays the assignment in each student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="383ce-109">权限</span><span class="sxs-lookup"><span data-stu-id="383ce-109">Permissions</span></span>
<span data-ttu-id="383ce-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="383ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="383ce-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="383ce-112">Permission type</span></span>      | <span data-ttu-id="383ce-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="383ce-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="383ce-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="383ce-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="383ce-115">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="383ce-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="383ce-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="383ce-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="383ce-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="383ce-117">Not supported.</span></span>  |
|<span data-ttu-id="383ce-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="383ce-118">Application</span></span> | <span data-ttu-id="383ce-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="383ce-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="383ce-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="383ce-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="383ce-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="383ce-121">Request headers</span></span>
| <span data-ttu-id="383ce-122">标头</span><span class="sxs-lookup"><span data-stu-id="383ce-122">Header</span></span>       | <span data-ttu-id="383ce-123">值</span><span class="sxs-lookup"><span data-stu-id="383ce-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="383ce-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="383ce-124">Authorization</span></span>  | <span data-ttu-id="383ce-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="383ce-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="383ce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="383ce-127">Request body</span></span>
<span data-ttu-id="383ce-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="383ce-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="383ce-129">响应</span><span class="sxs-lookup"><span data-stu-id="383ce-129">Response</span></span>
<span data-ttu-id="383ce-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="383ce-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="383ce-132">示例</span><span class="sxs-lookup"><span data-stu-id="383ce-132">Example</span></span>
<span data-ttu-id="383ce-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="383ce-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="383ce-134">请求</span><span class="sxs-lookup"><span data-stu-id="383ce-134">Request</span></span>
<span data-ttu-id="383ce-135">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="383ce-135">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="383ce-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="383ce-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "educationassignment_publish_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/publish
```
# <a name="c"></a>[<span data-ttu-id="383ce-137">C#</span><span class="sxs-lookup"><span data-stu-id="383ce-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="383ce-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="383ce-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="383ce-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="383ce-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="383ce-140">Java</span><span class="sxs-lookup"><span data-stu-id="383ce-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="383ce-141">响应</span><span class="sxs-lookup"><span data-stu-id="383ce-141">Response</span></span>
<span data-ttu-id="383ce-142">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="383ce-142">The following is an example of a response.</span></span> 

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
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


