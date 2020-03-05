---
title: 删除 educationAssignmentResource
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ab9bdc849988ac44e52370991bd20f9c51a6e04e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427254"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="2e001-103">删除 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="2e001-103">Delete educationAssignmentResource</span></span>

<span data-ttu-id="2e001-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2e001-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e001-105">从工作分配中删除资源。</span><span class="sxs-lookup"><span data-stu-id="2e001-105">Delete a resource from an assignment.</span></span> <span data-ttu-id="2e001-106">只有课堂中的教师才能删除资源。</span><span class="sxs-lookup"><span data-stu-id="2e001-106">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="2e001-107">向学生发布分配后，教师将无法删除标记为 "distributeToStudents" 的资源。</span><span class="sxs-lookup"><span data-stu-id="2e001-107">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="2e001-108">权限</span><span class="sxs-lookup"><span data-stu-id="2e001-108">Permissions</span></span>
<span data-ttu-id="2e001-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e001-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e001-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e001-111">Permission type</span></span>      | <span data-ttu-id="2e001-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e001-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e001-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e001-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="2e001-114">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="2e001-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2e001-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e001-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2e001-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e001-116">Not supported.</span></span>  |
|<span data-ttu-id="2e001-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e001-117">Application</span></span> | <span data-ttu-id="2e001-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e001-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2e001-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e001-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="2e001-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e001-120">Request headers</span></span>
| <span data-ttu-id="2e001-121">标头</span><span class="sxs-lookup"><span data-stu-id="2e001-121">Header</span></span>       | <span data-ttu-id="2e001-122">值</span><span class="sxs-lookup"><span data-stu-id="2e001-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e001-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e001-123">Authorization</span></span>  | <span data-ttu-id="2e001-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e001-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e001-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e001-126">Request body</span></span>
<span data-ttu-id="2e001-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2e001-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2e001-128">响应</span><span class="sxs-lookup"><span data-stu-id="2e001-128">Response</span></span>
<span data-ttu-id="2e001-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2e001-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e001-131">示例</span><span class="sxs-lookup"><span data-stu-id="2e001-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e001-132">请求</span><span class="sxs-lookup"><span data-stu-id="2e001-132">Request</span></span>
<span data-ttu-id="2e001-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2e001-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e001-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e001-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="2e001-135">C#</span><span class="sxs-lookup"><span data-stu-id="2e001-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e001-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e001-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e001-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e001-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e001-138">响应</span><span class="sxs-lookup"><span data-stu-id="2e001-138">Response</span></span>
<span data-ttu-id="2e001-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2e001-139">The following is an example of the response.</span></span> 


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
