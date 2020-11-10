---
title: 删除 outlookTask
description: 删除用户邮箱中的指定 Outlook 任务。
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 42dbfd011b9bc0bd50ef91049767c27016f0d9b9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951504"
---
# <a name="delete-outlooktask-deprecated"></a><span data-ttu-id="f136c-103">删除 outlookTask (弃用) </span><span class="sxs-lookup"><span data-stu-id="f136c-103">Delete outlookTask (deprecated)</span></span>

<span data-ttu-id="f136c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f136c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="f136c-105">删除用户邮箱中的指定 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="f136c-105">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="f136c-106">权限</span><span class="sxs-lookup"><span data-stu-id="f136c-106">Permissions</span></span>

<span data-ttu-id="f136c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f136c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f136c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f136c-109">Permission type</span></span>      | <span data-ttu-id="f136c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f136c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f136c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f136c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f136c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f136c-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f136c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f136c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f136c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f136c-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f136c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f136c-115">Application</span></span> | <span data-ttu-id="f136c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f136c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f136c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f136c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f136c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f136c-118">Request headers</span></span>

| <span data-ttu-id="f136c-119">名称</span><span class="sxs-lookup"><span data-stu-id="f136c-119">Name</span></span>       | <span data-ttu-id="f136c-120">说明</span><span class="sxs-lookup"><span data-stu-id="f136c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f136c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f136c-121">Authorization</span></span>  | <span data-ttu-id="f136c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f136c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f136c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f136c-124">Request body</span></span>

<span data-ttu-id="f136c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f136c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f136c-126">响应</span><span class="sxs-lookup"><span data-stu-id="f136c-126">Response</span></span>

<span data-ttu-id="f136c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f136c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f136c-129">示例</span><span class="sxs-lookup"><span data-stu-id="f136c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f136c-130">请求</span><span class="sxs-lookup"><span data-stu-id="f136c-130">Request</span></span>

<span data-ttu-id="f136c-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f136c-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f136c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f136c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=
```
# <a name="c"></a>[<span data-ttu-id="f136c-133">C#</span><span class="sxs-lookup"><span data-stu-id="f136c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f136c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f136c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f136c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f136c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f136c-136">Java</span><span class="sxs-lookup"><span data-stu-id="f136c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f136c-137">响应</span><span class="sxs-lookup"><span data-stu-id="f136c-137">Response</span></span>

<span data-ttu-id="f136c-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f136c-138">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


