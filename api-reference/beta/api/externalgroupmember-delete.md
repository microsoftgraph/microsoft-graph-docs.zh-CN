---
title: 删除 externalGroupMember
description: 删除 externalGroupMember 对象。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b6a6c79288d2eee9ff4ef2cbb0a9d200a6735050
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954613"
---
# <a name="delete-externalgroupmember"></a><span data-ttu-id="edd34-103">删除 externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="edd34-103">Delete externalGroupMember</span></span>

<span data-ttu-id="edd34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edd34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edd34-105">删除 [externalGroupMember](../resources/externalgroupmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edd34-105">Delete an [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="edd34-106">权限</span><span class="sxs-lookup"><span data-stu-id="edd34-106">Permissions</span></span>

<span data-ttu-id="edd34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edd34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="edd34-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="edd34-109">Permission type</span></span>                        | <span data-ttu-id="edd34-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="edd34-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="edd34-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edd34-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="edd34-112">不支持</span><span class="sxs-lookup"><span data-stu-id="edd34-112">Not supported</span></span>                               |
| <span data-ttu-id="edd34-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edd34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edd34-114">不支持</span><span class="sxs-lookup"><span data-stu-id="edd34-114">Not supported</span></span>                               |
| <span data-ttu-id="edd34-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="edd34-115">Application</span></span>                            | <span data-ttu-id="edd34-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edd34-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="edd34-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edd34-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}/members/{externalGroupMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="edd34-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="edd34-118">Request headers</span></span>

| <span data-ttu-id="edd34-119">名称</span><span class="sxs-lookup"><span data-stu-id="edd34-119">Name</span></span>          | <span data-ttu-id="edd34-120">说明</span><span class="sxs-lookup"><span data-stu-id="edd34-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="edd34-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="edd34-121">Authorization</span></span> | <span data-ttu-id="edd34-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="edd34-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="edd34-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="edd34-124">Request body</span></span>

<span data-ttu-id="edd34-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="edd34-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edd34-126">响应</span><span class="sxs-lookup"><span data-stu-id="edd34-126">Response</span></span>

<span data-ttu-id="edd34-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="edd34-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="edd34-128">示例</span><span class="sxs-lookup"><span data-stu-id="edd34-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="edd34-129">请求</span><span class="sxs-lookup"><span data-stu-id="edd34-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="edd34-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="edd34-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroupmember"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a
```
# <a name="c"></a>[<span data-ttu-id="edd34-131">C#</span><span class="sxs-lookup"><span data-stu-id="edd34-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroupmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edd34-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edd34-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroupmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edd34-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edd34-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroupmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edd34-134">Java</span><span class="sxs-lookup"><span data-stu-id="edd34-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroupmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="edd34-135">响应</span><span class="sxs-lookup"><span data-stu-id="edd34-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
