---
title: 删除 personCertification
description: 删除 personCertification 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9defbcc8505176c305626dc710b4ba4c13c634fa
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573955"
---
# <a name="delete-personcertification"></a><span data-ttu-id="7895a-103">删除 personCertification</span><span class="sxs-lookup"><span data-stu-id="7895a-103">Delete personCertification</span></span>
<span data-ttu-id="7895a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7895a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7895a-105">从用户配置文件 [中删除 personCertification](../resources/personcertification.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="7895a-105">Deletes a [personCertification](../resources/personcertification.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7895a-106">权限</span><span class="sxs-lookup"><span data-stu-id="7895a-106">Permissions</span></span>

<span data-ttu-id="7895a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7895a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7895a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7895a-109">Permission type</span></span>                        | <span data-ttu-id="7895a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7895a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="7895a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7895a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7895a-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7895a-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7895a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7895a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7895a-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7895a-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7895a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7895a-115">Application</span></span>                            | <span data-ttu-id="7895a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7895a-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="7895a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7895a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/certifications/{id}
DELETE /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7895a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7895a-118">Request headers</span></span>
|<span data-ttu-id="7895a-119">名称</span><span class="sxs-lookup"><span data-stu-id="7895a-119">Name</span></span>|<span data-ttu-id="7895a-120">说明</span><span class="sxs-lookup"><span data-stu-id="7895a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7895a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7895a-121">Authorization</span></span>|<span data-ttu-id="7895a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7895a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7895a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7895a-124">Request body</span></span>
<span data-ttu-id="7895a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7895a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7895a-126">响应</span><span class="sxs-lookup"><span data-stu-id="7895a-126">Response</span></span>

<span data-ttu-id="7895a-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7895a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7895a-128">示例</span><span class="sxs-lookup"><span data-stu-id="7895a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7895a-129">请求</span><span class="sxs-lookup"><span data-stu-id="7895a-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="7895a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7895a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personCertification"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/certifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="7895a-131">C#</span><span class="sxs-lookup"><span data-stu-id="7895a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7895a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7895a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7895a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7895a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="7895a-134">响应</span><span class="sxs-lookup"><span data-stu-id="7895a-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


