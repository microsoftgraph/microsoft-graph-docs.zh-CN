---
title: ediscoveryCase： close
description: 关闭电子数据展示案例。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 90b899cf526dbb54687d8b4a8825536f232ac631
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657057"
---
# <a name="ediscoverycase-close"></a><span data-ttu-id="5d64a-103">ediscoveryCase： close</span><span class="sxs-lookup"><span data-stu-id="5d64a-103">ediscoveryCase: close</span></span>

<span data-ttu-id="5d64a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d64a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d64a-105">关闭电子数据展示案例。</span><span class="sxs-lookup"><span data-stu-id="5d64a-105">Close an eDiscovery case.</span></span> <span data-ttu-id="5d64a-106">有关详细信息，请参阅["关闭案例"。](/microsoft-365/compliance/close-or-delete-case#close-a-case)</span><span class="sxs-lookup"><span data-stu-id="5d64a-106">For details, see [Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d64a-107">权限</span><span class="sxs-lookup"><span data-stu-id="5d64a-107">Permissions</span></span>

<span data-ttu-id="5d64a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d64a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d64a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d64a-110">Permission type</span></span>|<span data-ttu-id="5d64a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5d64a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d64a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d64a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5d64a-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="5d64a-113">User.Read</span></span>|
|<span data-ttu-id="5d64a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d64a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d64a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d64a-115">Not supported.</span></span>|
|<span data-ttu-id="5d64a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d64a-116">Application</span></span>|<span data-ttu-id="5d64a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d64a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d64a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d64a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/close
```

## <a name="request-headers"></a><span data-ttu-id="5d64a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d64a-119">Request headers</span></span>

|<span data-ttu-id="5d64a-120">名称</span><span class="sxs-lookup"><span data-stu-id="5d64a-120">Name</span></span>|<span data-ttu-id="5d64a-121">说明</span><span class="sxs-lookup"><span data-stu-id="5d64a-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5d64a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d64a-122">Authorization</span></span>|<span data-ttu-id="5d64a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d64a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d64a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d64a-125">Request body</span></span>

<span data-ttu-id="5d64a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d64a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d64a-127">响应</span><span class="sxs-lookup"><span data-stu-id="5d64a-127">Response</span></span>

<span data-ttu-id="5d64a-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5d64a-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5d64a-129">示例</span><span class="sxs-lookup"><span data-stu-id="5d64a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d64a-130">请求</span><span class="sxs-lookup"><span data-stu-id="5d64a-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5d64a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d64a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoverycase_close"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/close
```
# <a name="c"></a>[<span data-ttu-id="5d64a-132">C#</span><span class="sxs-lookup"><span data-stu-id="5d64a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-close-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d64a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d64a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-close-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d64a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d64a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-close-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d64a-135">Java</span><span class="sxs-lookup"><span data-stu-id="5d64a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-close-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d64a-136">响应</span><span class="sxs-lookup"><span data-stu-id="5d64a-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
