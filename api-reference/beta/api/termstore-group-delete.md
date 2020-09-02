---
title: 删除组
description: 删除组对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: fc013c512016c9ff683b0fe3f0e4c369141ba612
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330268"
---
# <a name="delete-groups"></a><span data-ttu-id="4e74a-103">删除组</span><span class="sxs-lookup"><span data-stu-id="4e74a-103">Delete groups</span></span>
<span data-ttu-id="4e74a-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="4e74a-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e74a-105">删除术语[库]中的[group](../resources/termstore-group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4e74a-105">Delete a [group](../resources/termstore-group.md) object in the term [store].</span></span>

## <a name="permissions"></a><span data-ttu-id="4e74a-106">权限</span><span class="sxs-lookup"><span data-stu-id="4e74a-106">Permissions</span></span>
<span data-ttu-id="4e74a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e74a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e74a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e74a-109">Permission type</span></span>|<span data-ttu-id="4e74a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4e74a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e74a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e74a-111">Delegated (work or school account)</span></span> |<span data-ttu-id="4e74a-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e74a-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="4e74a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e74a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e74a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e74a-114">Not supported.</span></span>    |
|<span data-ttu-id="4e74a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e74a-115">Application</span></span> | <span data-ttu-id="4e74a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e74a-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="4e74a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e74a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="4e74a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e74a-118">Request headers</span></span>
|<span data-ttu-id="4e74a-119">名称</span><span class="sxs-lookup"><span data-stu-id="4e74a-119">Name</span></span>|<span data-ttu-id="4e74a-120">说明</span><span class="sxs-lookup"><span data-stu-id="4e74a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4e74a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e74a-121">Authorization</span></span>|<span data-ttu-id="4e74a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e74a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e74a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e74a-124">Request body</span></span>
<span data-ttu-id="4e74a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e74a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e74a-126">响应</span><span class="sxs-lookup"><span data-stu-id="4e74a-126">Response</span></span>

<span data-ttu-id="4e74a-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4e74a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4e74a-128">示例</span><span class="sxs-lookup"><span data-stu-id="4e74a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4e74a-129">请求</span><span class="sxs-lookup"><span data-stu-id="4e74a-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4e74a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e74a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_from_store"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="4e74a-131">C#</span><span class="sxs-lookup"><span data-stu-id="4e74a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-from-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e74a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e74a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-from-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e74a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e74a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-from-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4e74a-134">响应</span><span class="sxs-lookup"><span data-stu-id="4e74a-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.store]: ../resources/termstore-store.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termGroup",
  "suppressions": [
  ]
}
-->
