---
title: 删除 itemPublication
description: 删除一个 itemPublication 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6e63ef86de454e63f6b90f4b9bf4ea79cfeb1222
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969889"
---
# <a name="delete-itempublication"></a><span data-ttu-id="b3cd0-103">删除 itemPublication</span><span class="sxs-lookup"><span data-stu-id="b3cd0-103">Delete itemPublication</span></span>

<span data-ttu-id="b3cd0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3cd0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3cd0-105">删除一个 [itemPublication](../resources/itempublication.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3cd0-105">Deletes an [itemPublication](../resources/itempublication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3cd0-106">权限</span><span class="sxs-lookup"><span data-stu-id="b3cd0-106">Permissions</span></span>

<span data-ttu-id="b3cd0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3cd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3cd0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3cd0-109">Permission type</span></span>                        | <span data-ttu-id="b3cd0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3cd0-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b3cd0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3cd0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3cd0-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="b3cd0-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b3cd0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3cd0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3cd0-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="b3cd0-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b3cd0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3cd0-115">Application</span></span>                            | <span data-ttu-id="b3cd0-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3cd0-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b3cd0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3cd0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/publications/{id}
DELETE /users/{id | userPrincipalName}/profile/publications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b3cd0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3cd0-118">Request headers</span></span>
|<span data-ttu-id="b3cd0-119">名称</span><span class="sxs-lookup"><span data-stu-id="b3cd0-119">Name</span></span>|<span data-ttu-id="b3cd0-120">说明</span><span class="sxs-lookup"><span data-stu-id="b3cd0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b3cd0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3cd0-121">Authorization</span></span>|<span data-ttu-id="b3cd0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3cd0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3cd0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3cd0-124">Request body</span></span>
<span data-ttu-id="b3cd0-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3cd0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3cd0-126">响应</span><span class="sxs-lookup"><span data-stu-id="b3cd0-126">Response</span></span>

<span data-ttu-id="b3cd0-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b3cd0-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b3cd0-128">示例</span><span class="sxs-lookup"><span data-stu-id="b3cd0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3cd0-129">请求</span><span class="sxs-lookup"><span data-stu-id="b3cd0-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="b3cd0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3cd0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemPublication"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/profile/publications/{id}
```
# <a name="c"></a>[<span data-ttu-id="b3cd0-131">C#</span><span class="sxs-lookup"><span data-stu-id="b3cd0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itempublication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3cd0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3cd0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itempublication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3cd0-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3cd0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itempublication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3cd0-134">Java</span><span class="sxs-lookup"><span data-stu-id="b3cd0-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-itempublication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b3cd0-135">响应</span><span class="sxs-lookup"><span data-stu-id="b3cd0-135">Response</span></span>
<span data-ttu-id="b3cd0-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b3cd0-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


