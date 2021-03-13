---
title: case： reopen
description: 重新打开已关闭电子数据展示案例。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2b220e42a6bc7bf69fee34b69bb9d40ed16137de
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773716"
---
# <a name="case-reopen"></a><span data-ttu-id="48a98-103">case： reopen</span><span class="sxs-lookup"><span data-stu-id="48a98-103">case: reopen</span></span>

<span data-ttu-id="48a98-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="48a98-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48a98-105">重新打开已关闭电子数据展示案例。</span><span class="sxs-lookup"><span data-stu-id="48a98-105">Reopen an eDiscovery case that was closed.</span></span> <span data-ttu-id="48a98-106">有关详细信息，请参阅 [重新打开已关闭的案例](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case)。</span><span class="sxs-lookup"><span data-stu-id="48a98-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="48a98-107">权限</span><span class="sxs-lookup"><span data-stu-id="48a98-107">Permissions</span></span>

<span data-ttu-id="48a98-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48a98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48a98-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="48a98-110">Permission type</span></span>|<span data-ttu-id="48a98-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48a98-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48a98-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48a98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48a98-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48a98-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="48a98-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48a98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48a98-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="48a98-115">Not supported.</span></span>|
|<span data-ttu-id="48a98-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="48a98-116">Application</span></span>|<span data-ttu-id="48a98-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="48a98-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48a98-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48a98-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reopen
```

## <a name="request-headers"></a><span data-ttu-id="48a98-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="48a98-119">Request headers</span></span>

|<span data-ttu-id="48a98-120">名称</span><span class="sxs-lookup"><span data-stu-id="48a98-120">Name</span></span>|<span data-ttu-id="48a98-121">说明</span><span class="sxs-lookup"><span data-stu-id="48a98-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="48a98-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48a98-122">Authorization</span></span>|<span data-ttu-id="48a98-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="48a98-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48a98-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="48a98-125">Request body</span></span>

<span data-ttu-id="48a98-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="48a98-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48a98-127">响应</span><span class="sxs-lookup"><span data-stu-id="48a98-127">Response</span></span>

<span data-ttu-id="48a98-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="48a98-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="48a98-129">示例</span><span class="sxs-lookup"><span data-stu-id="48a98-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48a98-130">请求</span><span class="sxs-lookup"><span data-stu-id="48a98-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="48a98-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a98-131">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "case_reopen"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen
```
# <a name="c"></a>[<span data-ttu-id="48a98-132">C#</span><span class="sxs-lookup"><span data-stu-id="48a98-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/case-reopen-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48a98-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48a98-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/case-reopen-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48a98-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48a98-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/case-reopen-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48a98-135">Java</span><span class="sxs-lookup"><span data-stu-id="48a98-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/case-reopen-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="48a98-136">响应</span><span class="sxs-lookup"><span data-stu-id="48a98-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
