---
title: 删除 personAnnotation
description: 删除 personAnnotation 对象。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 16993d5919c0d588710ac2835cc2bd0f4f46a1a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774213"
---
# <a name="delete-personannotation"></a><span data-ttu-id="169d8-103">删除 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="169d8-103">Delete personAnnotation</span></span>
<span data-ttu-id="169d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="169d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="169d8-105">从用户配置文件中删除 [personAnnotation](../resources/personannotation.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="169d8-105">Deletes a [personAnnotation](../resources/personannotation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="169d8-106">权限</span><span class="sxs-lookup"><span data-stu-id="169d8-106">Permissions</span></span>

<span data-ttu-id="169d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="169d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="169d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="169d8-109">Permission type</span></span>                        | <span data-ttu-id="169d8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="169d8-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="169d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="169d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="169d8-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="169d8-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="169d8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="169d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="169d8-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="169d8-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="169d8-115">Application</span><span class="sxs-lookup"><span data-stu-id="169d8-115">Application</span></span>                            | <span data-ttu-id="169d8-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="169d8-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="169d8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="169d8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/notes/{id}
DELETE /users/{id | userPrincipalName}/profile/notes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="169d8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="169d8-118">Request headers</span></span>
|<span data-ttu-id="169d8-119">名称</span><span class="sxs-lookup"><span data-stu-id="169d8-119">Name</span></span>|<span data-ttu-id="169d8-120">说明</span><span class="sxs-lookup"><span data-stu-id="169d8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="169d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="169d8-121">Authorization</span></span>|<span data-ttu-id="169d8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="169d8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="169d8-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="169d8-124">Request body</span></span>
<span data-ttu-id="169d8-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="169d8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="169d8-126">响应</span><span class="sxs-lookup"><span data-stu-id="169d8-126">Response</span></span>

<span data-ttu-id="169d8-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="169d8-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="169d8-128">示例</span><span class="sxs-lookup"><span data-stu-id="169d8-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="169d8-129">请求</span><span class="sxs-lookup"><span data-stu-id="169d8-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="169d8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="169d8-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personannotation"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/notes/{id}
```
# <a name="c"></a>[<span data-ttu-id="169d8-131">C#</span><span class="sxs-lookup"><span data-stu-id="169d8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personannotation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="169d8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="169d8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personannotation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="169d8-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="169d8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personannotation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="169d8-134">Java</span><span class="sxs-lookup"><span data-stu-id="169d8-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-personannotation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="169d8-135">响应</span><span class="sxs-lookup"><span data-stu-id="169d8-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


