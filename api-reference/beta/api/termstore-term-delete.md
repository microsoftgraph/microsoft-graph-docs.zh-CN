---
title: 删除术语
description: 删除术语对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0bfa073025dc2ecfd3399d96c89390841049670a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972283"
---
# <a name="delete-term"></a><span data-ttu-id="5d51e-103">删除术语</span><span class="sxs-lookup"><span data-stu-id="5d51e-103">Delete term</span></span>
<span data-ttu-id="5d51e-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="5d51e-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d51e-105">删除 [术语](../resources/termstore-term.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d51e-105">Delete a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d51e-106">权限</span><span class="sxs-lookup"><span data-stu-id="5d51e-106">Permissions</span></span>
<span data-ttu-id="5d51e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d51e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d51e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d51e-109">Permission type</span></span>|<span data-ttu-id="5d51e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5d51e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d51e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d51e-111">Delegated (work or school account)</span></span> |<span data-ttu-id="5d51e-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d51e-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="5d51e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d51e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d51e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d51e-114">Not supported.</span></span>    |
|<span data-ttu-id="5d51e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d51e-115">Application</span></span> | <span data-ttu-id="5d51e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d51e-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="5d51e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d51e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="5d51e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d51e-118">Request headers</span></span>
|<span data-ttu-id="5d51e-119">名称</span><span class="sxs-lookup"><span data-stu-id="5d51e-119">Name</span></span>|<span data-ttu-id="5d51e-120">说明</span><span class="sxs-lookup"><span data-stu-id="5d51e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5d51e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d51e-121">Authorization</span></span>|<span data-ttu-id="5d51e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d51e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d51e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d51e-124">Request body</span></span>
<span data-ttu-id="5d51e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d51e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d51e-126">响应</span><span class="sxs-lookup"><span data-stu-id="5d51e-126">Response</span></span>

<span data-ttu-id="5d51e-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5d51e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5d51e-128">示例</span><span class="sxs-lookup"><span data-stu-id="5d51e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d51e-129">请求</span><span class="sxs-lookup"><span data-stu-id="5d51e-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5d51e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d51e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_term"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="5d51e-131">C#</span><span class="sxs-lookup"><span data-stu-id="5d51e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d51e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d51e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d51e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d51e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d51e-134">Java</span><span class="sxs-lookup"><span data-stu-id="5d51e-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-term-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5d51e-135">响应</span><span class="sxs-lookup"><span data-stu-id="5d51e-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete term",
  "suppressions": [
  ]
}
-->


