---
title: 删除 externalGroup
description: 删除 externalGroup 对象。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a039ab9969766a6fa1716c481c0d74f5b8bf125d
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873183"
---
# <a name="delete-externalgroup"></a><span data-ttu-id="ec65c-103">删除 externalGroup</span><span class="sxs-lookup"><span data-stu-id="ec65c-103">Delete externalGroup</span></span>

<span data-ttu-id="ec65c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec65c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec65c-105">删除 [externalGroup](../resources/externalgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec65c-105">Delete an [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec65c-106">权限</span><span class="sxs-lookup"><span data-stu-id="ec65c-106">Permissions</span></span>

<span data-ttu-id="ec65c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec65c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec65c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec65c-109">Permission type</span></span>                        | <span data-ttu-id="ec65c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec65c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ec65c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec65c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec65c-112">不支持</span><span class="sxs-lookup"><span data-stu-id="ec65c-112">Not supported</span></span>                               |
| <span data-ttu-id="ec65c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec65c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec65c-114">不支持</span><span class="sxs-lookup"><span data-stu-id="ec65c-114">Not supported</span></span>                               |
| <span data-ttu-id="ec65c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec65c-115">Application</span></span>                            | <span data-ttu-id="ec65c-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec65c-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="ec65c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec65c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="ec65c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec65c-118">Request headers</span></span>

| <span data-ttu-id="ec65c-119">名称</span><span class="sxs-lookup"><span data-stu-id="ec65c-119">Name</span></span>          | <span data-ttu-id="ec65c-120">说明</span><span class="sxs-lookup"><span data-stu-id="ec65c-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ec65c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec65c-121">Authorization</span></span> | <span data-ttu-id="ec65c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec65c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec65c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec65c-124">Request body</span></span>

<span data-ttu-id="ec65c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec65c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec65c-126">响应</span><span class="sxs-lookup"><span data-stu-id="ec65c-126">Response</span></span>

<span data-ttu-id="ec65c-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ec65c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ec65c-128">示例</span><span class="sxs-lookup"><span data-stu-id="ec65c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec65c-129">请求</span><span class="sxs-lookup"><span data-stu-id="ec65c-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ec65c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec65c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```
# <a name="c"></a>[<span data-ttu-id="ec65c-131">C#</span><span class="sxs-lookup"><span data-stu-id="ec65c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec65c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec65c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec65c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec65c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec65c-134">Java</span><span class="sxs-lookup"><span data-stu-id="ec65c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="ec65c-135">响应</span><span class="sxs-lookup"><span data-stu-id="ec65c-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
