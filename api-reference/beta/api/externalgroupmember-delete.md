---
title: 删除 externalGroupMember
description: 删除 externalGroupMember 对象。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 24bfa2da5277192f4f14e828a7e6ea2d5b5d9ce1
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873169"
---
# <a name="delete-externalgroupmember"></a><span data-ttu-id="36964-103">删除 externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="36964-103">Delete externalGroupMember</span></span>

<span data-ttu-id="36964-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36964-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36964-105">删除 [externalGroupMember](../resources/externalgroupmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36964-105">Delete an [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="36964-106">权限</span><span class="sxs-lookup"><span data-stu-id="36964-106">Permissions</span></span>

<span data-ttu-id="36964-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36964-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="36964-109">Permission type</span></span>                        | <span data-ttu-id="36964-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36964-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36964-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36964-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="36964-112">不支持</span><span class="sxs-lookup"><span data-stu-id="36964-112">Not supported</span></span>                               |
| <span data-ttu-id="36964-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36964-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36964-114">不支持</span><span class="sxs-lookup"><span data-stu-id="36964-114">Not supported</span></span>                               |
| <span data-ttu-id="36964-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="36964-115">Application</span></span>                            | <span data-ttu-id="36964-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36964-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="36964-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36964-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}/members/{externalGroupMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="36964-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="36964-118">Request headers</span></span>

| <span data-ttu-id="36964-119">名称</span><span class="sxs-lookup"><span data-stu-id="36964-119">Name</span></span>          | <span data-ttu-id="36964-120">说明</span><span class="sxs-lookup"><span data-stu-id="36964-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="36964-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36964-121">Authorization</span></span> | <span data-ttu-id="36964-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36964-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36964-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="36964-124">Request body</span></span>

<span data-ttu-id="36964-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36964-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36964-126">响应</span><span class="sxs-lookup"><span data-stu-id="36964-126">Response</span></span>

<span data-ttu-id="36964-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="36964-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="36964-128">示例</span><span class="sxs-lookup"><span data-stu-id="36964-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36964-129">请求</span><span class="sxs-lookup"><span data-stu-id="36964-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36964-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="36964-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroupmember"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a
```
# <a name="c"></a>[<span data-ttu-id="36964-131">C#</span><span class="sxs-lookup"><span data-stu-id="36964-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroupmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36964-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36964-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroupmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36964-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36964-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroupmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36964-134">Java</span><span class="sxs-lookup"><span data-stu-id="36964-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroupmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="36964-135">响应</span><span class="sxs-lookup"><span data-stu-id="36964-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
