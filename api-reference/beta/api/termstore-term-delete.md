---
title: 删除术语
description: 删除术语对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 706ad5b9457014de236485f526db994dd8a29866
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874373"
---
# <a name="delete-term"></a><span data-ttu-id="e8730-103">删除术语</span><span class="sxs-lookup"><span data-stu-id="e8730-103">Delete term</span></span>
<span data-ttu-id="e8730-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="e8730-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8730-105">删除 [术语](../resources/termstore-term.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8730-105">Delete a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8730-106">权限</span><span class="sxs-lookup"><span data-stu-id="e8730-106">Permissions</span></span>
<span data-ttu-id="e8730-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8730-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8730-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8730-109">Permission type</span></span>|<span data-ttu-id="e8730-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8730-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8730-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8730-111">Delegated (work or school account)</span></span> |<span data-ttu-id="e8730-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8730-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="e8730-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8730-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8730-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8730-114">Not supported.</span></span>    |
|<span data-ttu-id="e8730-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8730-115">Application</span></span> | <span data-ttu-id="e8730-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8730-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="e8730-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8730-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="e8730-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8730-118">Request headers</span></span>
|<span data-ttu-id="e8730-119">名称</span><span class="sxs-lookup"><span data-stu-id="e8730-119">Name</span></span>|<span data-ttu-id="e8730-120">说明</span><span class="sxs-lookup"><span data-stu-id="e8730-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e8730-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8730-121">Authorization</span></span>|<span data-ttu-id="e8730-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8730-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8730-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8730-124">Request body</span></span>
<span data-ttu-id="e8730-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8730-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8730-126">响应</span><span class="sxs-lookup"><span data-stu-id="e8730-126">Response</span></span>

<span data-ttu-id="e8730-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e8730-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e8730-128">示例</span><span class="sxs-lookup"><span data-stu-id="e8730-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8730-129">请求</span><span class="sxs-lookup"><span data-stu-id="e8730-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e8730-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8730-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_term"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="e8730-131">C#</span><span class="sxs-lookup"><span data-stu-id="e8730-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8730-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8730-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8730-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8730-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8730-134">Java</span><span class="sxs-lookup"><span data-stu-id="e8730-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-term-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e8730-135">响应</span><span class="sxs-lookup"><span data-stu-id="e8730-135">Response</span></span>
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


