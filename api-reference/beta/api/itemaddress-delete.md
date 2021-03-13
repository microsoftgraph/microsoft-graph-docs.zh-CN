---
title: 删除 itemAddress
description: 删除 itemAddress 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1469633fd4cff278914bc4aa6cb6a757fd20c36f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774714"
---
# <a name="delete-itemaddress"></a><span data-ttu-id="65158-103">删除 itemAddress</span><span class="sxs-lookup"><span data-stu-id="65158-103">Delete itemAddress</span></span>
<span data-ttu-id="65158-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65158-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65158-105">删除 [itemAddress](../resources/itemaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65158-105">Deletes an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="65158-106">权限</span><span class="sxs-lookup"><span data-stu-id="65158-106">Permissions</span></span>

<span data-ttu-id="65158-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65158-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65158-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65158-109">Permission type</span></span>                        | <span data-ttu-id="65158-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65158-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="65158-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65158-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65158-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65158-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="65158-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65158-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65158-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65158-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="65158-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="65158-115">Application</span></span>                            | <span data-ttu-id="65158-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65158-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="65158-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65158-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/addresses/{id}
DELETE /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="request-headers"></a><span data-ttu-id="65158-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="65158-118">Request headers</span></span>
|<span data-ttu-id="65158-119">名称</span><span class="sxs-lookup"><span data-stu-id="65158-119">Name</span></span>|<span data-ttu-id="65158-120">说明</span><span class="sxs-lookup"><span data-stu-id="65158-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65158-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65158-121">Authorization</span></span>|<span data-ttu-id="65158-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65158-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65158-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="65158-124">Request body</span></span>
<span data-ttu-id="65158-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65158-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65158-126">响应</span><span class="sxs-lookup"><span data-stu-id="65158-126">Response</span></span>

<span data-ttu-id="65158-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="65158-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="65158-128">示例</span><span class="sxs-lookup"><span data-stu-id="65158-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65158-129">请求</span><span class="sxs-lookup"><span data-stu-id="65158-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="65158-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="65158-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemaddress"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/addresses/{id}
```
# <a name="c"></a>[<span data-ttu-id="65158-131">C#</span><span class="sxs-lookup"><span data-stu-id="65158-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itemaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65158-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65158-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itemaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65158-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65158-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itemaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65158-134">Java</span><span class="sxs-lookup"><span data-stu-id="65158-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-itemaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="65158-135">响应</span><span class="sxs-lookup"><span data-stu-id="65158-135">Response</span></span>
<span data-ttu-id="65158-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="65158-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


