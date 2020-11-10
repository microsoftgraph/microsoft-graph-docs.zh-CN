---
title: 删除集
description: 删除集对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 28ed1e580c13ce675e09f6b892cbd4989e56d664
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980082"
---
# <a name="delete-set"></a><span data-ttu-id="113b1-103">删除集</span><span class="sxs-lookup"><span data-stu-id="113b1-103">Delete set</span></span>
<span data-ttu-id="113b1-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="113b1-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="113b1-105">删除 [集](../resources/termstore-set.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="113b1-105">Delete a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="113b1-106">权限</span><span class="sxs-lookup"><span data-stu-id="113b1-106">Permissions</span></span>
<span data-ttu-id="113b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="113b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="113b1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="113b1-109">Permission type</span></span>|<span data-ttu-id="113b1-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="113b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="113b1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="113b1-111">Delegated (work or school account)</span></span> |<span data-ttu-id="113b1-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="113b1-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="113b1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="113b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="113b1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="113b1-114">Not supported.</span></span>    |
|<span data-ttu-id="113b1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="113b1-115">Application</span></span> | <span data-ttu-id="113b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="113b1-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="113b1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="113b1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="113b1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="113b1-118">Request headers</span></span>
|<span data-ttu-id="113b1-119">名称</span><span class="sxs-lookup"><span data-stu-id="113b1-119">Name</span></span>|<span data-ttu-id="113b1-120">说明</span><span class="sxs-lookup"><span data-stu-id="113b1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="113b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="113b1-121">Authorization</span></span>|<span data-ttu-id="113b1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="113b1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="113b1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="113b1-124">Request body</span></span>
<span data-ttu-id="113b1-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="113b1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="113b1-126">响应</span><span class="sxs-lookup"><span data-stu-id="113b1-126">Response</span></span>

<span data-ttu-id="113b1-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="113b1-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="113b1-128">示例</span><span class="sxs-lookup"><span data-stu-id="113b1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="113b1-129">请求</span><span class="sxs-lookup"><span data-stu-id="113b1-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="113b1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="113b1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_set"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}
```
# <a name="c"></a>[<span data-ttu-id="113b1-131">C#</span><span class="sxs-lookup"><span data-stu-id="113b1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="113b1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="113b1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="113b1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="113b1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="113b1-134">Java</span><span class="sxs-lookup"><span data-stu-id="113b1-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-set-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="113b1-135">响应</span><span class="sxs-lookup"><span data-stu-id="113b1-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termSet",
  "suppressions": [
  ]
}
-->


