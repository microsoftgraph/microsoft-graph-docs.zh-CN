---
title: 删除 personCertification
description: 删除一个 personCertification 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: da30a5b3646dc5b72ccc726740d6ad7f076490d1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812949"
---
# <a name="delete-personcertification"></a><span data-ttu-id="4eb20-103">删除 personCertification</span><span class="sxs-lookup"><span data-stu-id="4eb20-103">Delete personCertification</span></span>
<span data-ttu-id="4eb20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eb20-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4eb20-105">从用户的[配置文件](../resources/profile.md)中删除[personCertification](../resources/personcertification.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4eb20-105">Deletes a [personCertification](../resources/personcertification.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4eb20-106">权限</span><span class="sxs-lookup"><span data-stu-id="4eb20-106">Permissions</span></span>

<span data-ttu-id="4eb20-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4eb20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4eb20-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4eb20-109">Permission type</span></span>                        | <span data-ttu-id="4eb20-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4eb20-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="4eb20-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4eb20-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4eb20-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="4eb20-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4eb20-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4eb20-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eb20-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="4eb20-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4eb20-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4eb20-115">Application</span></span>                            | <span data-ttu-id="4eb20-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eb20-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="4eb20-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4eb20-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/certifications/{id}
DELETE /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4eb20-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4eb20-118">Request headers</span></span>
|<span data-ttu-id="4eb20-119">名称</span><span class="sxs-lookup"><span data-stu-id="4eb20-119">Name</span></span>|<span data-ttu-id="4eb20-120">说明</span><span class="sxs-lookup"><span data-stu-id="4eb20-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4eb20-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eb20-121">Authorization</span></span>|<span data-ttu-id="4eb20-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4eb20-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eb20-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4eb20-124">Request body</span></span>
<span data-ttu-id="4eb20-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4eb20-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eb20-126">响应</span><span class="sxs-lookup"><span data-stu-id="4eb20-126">Response</span></span>

<span data-ttu-id="4eb20-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4eb20-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4eb20-128">示例</span><span class="sxs-lookup"><span data-stu-id="4eb20-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4eb20-129">请求</span><span class="sxs-lookup"><span data-stu-id="4eb20-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="4eb20-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4eb20-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personCertification"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/certifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="4eb20-131">C#</span><span class="sxs-lookup"><span data-stu-id="4eb20-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4eb20-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4eb20-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4eb20-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4eb20-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4eb20-134">响应</span><span class="sxs-lookup"><span data-stu-id="4eb20-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
