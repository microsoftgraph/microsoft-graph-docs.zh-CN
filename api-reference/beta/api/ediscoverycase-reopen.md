---
title: ediscoveryCase：reopen
description: 重新打开已关闭电子数据展示案例。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 256dba8a09e2be3be20aadd4e2c8e9927f2b20df
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657084"
---
# <a name="ediscoverycase-reopen"></a><span data-ttu-id="eb441-103">ediscoveryCase：reopen</span><span class="sxs-lookup"><span data-stu-id="eb441-103">ediscoveryCase: reopen</span></span>

<span data-ttu-id="eb441-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb441-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb441-105">重新打开已关闭电子数据展示案例。</span><span class="sxs-lookup"><span data-stu-id="eb441-105">Reopen an eDiscovery case that was closed.</span></span> <span data-ttu-id="eb441-106">有关详细信息，请参阅重新打开 [关闭的大小写](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case)。</span><span class="sxs-lookup"><span data-stu-id="eb441-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb441-107">权限</span><span class="sxs-lookup"><span data-stu-id="eb441-107">Permissions</span></span>
<span data-ttu-id="eb441-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb441-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb441-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb441-110">Permission type</span></span>|<span data-ttu-id="eb441-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eb441-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb441-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb441-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb441-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="eb441-113">User.Read</span></span>|
|<span data-ttu-id="eb441-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb441-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb441-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb441-115">Not supported.</span></span>|
|<span data-ttu-id="eb441-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb441-116">Application</span></span>|<span data-ttu-id="eb441-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb441-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb441-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb441-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/reopen
```

## <a name="request-headers"></a><span data-ttu-id="eb441-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb441-119">Request headers</span></span>

|<span data-ttu-id="eb441-120">名称</span><span class="sxs-lookup"><span data-stu-id="eb441-120">Name</span></span>|<span data-ttu-id="eb441-121">说明</span><span class="sxs-lookup"><span data-stu-id="eb441-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eb441-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb441-122">Authorization</span></span>|<span data-ttu-id="eb441-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb441-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb441-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb441-125">Request body</span></span>

<span data-ttu-id="eb441-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb441-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb441-127">响应</span><span class="sxs-lookup"><span data-stu-id="eb441-127">Response</span></span>

<span data-ttu-id="eb441-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eb441-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="eb441-129">示例</span><span class="sxs-lookup"><span data-stu-id="eb441-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb441-130">请求</span><span class="sxs-lookup"><span data-stu-id="eb441-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eb441-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb441-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoverycase_reopen"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen
```
# <a name="c"></a>[<span data-ttu-id="eb441-132">C#</span><span class="sxs-lookup"><span data-stu-id="eb441-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-reopen-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb441-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb441-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-reopen-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb441-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb441-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-reopen-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb441-135">Java</span><span class="sxs-lookup"><span data-stu-id="eb441-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-reopen-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb441-136">响应</span><span class="sxs-lookup"><span data-stu-id="eb441-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
