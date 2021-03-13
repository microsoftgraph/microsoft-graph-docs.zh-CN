---
title: 删除 itemPatent
description: 删除 itemPatent 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4c819a4ca1bb50a572fbbe593a7ec951714cf4cc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776275"
---
# <a name="delete-itempatent"></a><span data-ttu-id="cb938-103">删除 itemPatent</span><span class="sxs-lookup"><span data-stu-id="cb938-103">Delete itemPatent</span></span>

<span data-ttu-id="cb938-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb938-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb938-105">删除 [itemPatent](../resources/itempatent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb938-105">Deletes an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb938-106">权限</span><span class="sxs-lookup"><span data-stu-id="cb938-106">Permissions</span></span>

<span data-ttu-id="cb938-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb938-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb938-109">Permission type</span></span>                        | <span data-ttu-id="cb938-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb938-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="cb938-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb938-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb938-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb938-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="cb938-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb938-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb938-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb938-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="cb938-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb938-115">Application</span></span>                            | <span data-ttu-id="cb938-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb938-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="cb938-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb938-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/patents/{id}
DELETE /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cb938-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb938-118">Request headers</span></span>
|<span data-ttu-id="cb938-119">名称</span><span class="sxs-lookup"><span data-stu-id="cb938-119">Name</span></span>|<span data-ttu-id="cb938-120">说明</span><span class="sxs-lookup"><span data-stu-id="cb938-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb938-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb938-121">Authorization</span></span>|<span data-ttu-id="cb938-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb938-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb938-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb938-124">Request body</span></span>
<span data-ttu-id="cb938-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb938-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb938-126">响应</span><span class="sxs-lookup"><span data-stu-id="cb938-126">Response</span></span>

<span data-ttu-id="cb938-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cb938-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cb938-128">示例</span><span class="sxs-lookup"><span data-stu-id="cb938-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb938-129">请求</span><span class="sxs-lookup"><span data-stu-id="cb938-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="cb938-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb938-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itempatent"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/patents/{id}
```
# <a name="c"></a>[<span data-ttu-id="cb938-131">C#</span><span class="sxs-lookup"><span data-stu-id="cb938-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itempatent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb938-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb938-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itempatent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb938-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb938-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itempatent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb938-134">Java</span><span class="sxs-lookup"><span data-stu-id="cb938-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-itempatent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="cb938-135">响应</span><span class="sxs-lookup"><span data-stu-id="cb938-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


