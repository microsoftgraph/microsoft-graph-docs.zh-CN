---
title: 删除 unifiedGroupSource
description: 删除 unifiedGroupSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 1e5145d3e067c92ce5faf8f9ddd6b7012bd19220
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872455"
---
# <a name="delete-unifiedgroupsource"></a><span data-ttu-id="cf9bf-103">删除 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="cf9bf-103">Delete unifiedGroupSource</span></span>

<span data-ttu-id="cf9bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf9bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf9bf-105">删除 [unifiedGroupSource](../resources/unifiedgroupsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cf9bf-105">Delete a [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf9bf-106">权限</span><span class="sxs-lookup"><span data-stu-id="cf9bf-106">Permissions</span></span>

<span data-ttu-id="cf9bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf9bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf9bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf9bf-109">Permission type</span></span>|<span data-ttu-id="cf9bf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf9bf-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf9bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf9bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf9bf-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="cf9bf-112">User.Read</span></span>|
|<span data-ttu-id="cf9bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf9bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf9bf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf9bf-114">Not supported.</span></span>|
|<span data-ttu-id="cf9bf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf9bf-115">Application</span></span>|<span data-ttu-id="cf9bf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf9bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf9bf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf9bf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633
```

## <a name="request-headers"></a><span data-ttu-id="cf9bf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf9bf-118">Request headers</span></span>

|<span data-ttu-id="cf9bf-119">名称</span><span class="sxs-lookup"><span data-stu-id="cf9bf-119">Name</span></span>|<span data-ttu-id="cf9bf-120">说明</span><span class="sxs-lookup"><span data-stu-id="cf9bf-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cf9bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf9bf-121">Authorization</span></span>|<span data-ttu-id="cf9bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf9bf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf9bf-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf9bf-124">Request body</span></span>

<span data-ttu-id="cf9bf-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf9bf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf9bf-126">响应</span><span class="sxs-lookup"><span data-stu-id="cf9bf-126">Response</span></span>

<span data-ttu-id="cf9bf-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cf9bf-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cf9bf-128">示例</span><span class="sxs-lookup"><span data-stu-id="cf9bf-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf9bf-129">请求</span><span class="sxs-lookup"><span data-stu-id="cf9bf-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cf9bf-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf9bf-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedgroupsource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}
```
# <a name="c"></a>[<span data-ttu-id="cf9bf-131">C#</span><span class="sxs-lookup"><span data-stu-id="cf9bf-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedgroupsource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf9bf-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf9bf-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedgroupsource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf9bf-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf9bf-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedgroupsource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf9bf-134">Java</span><span class="sxs-lookup"><span data-stu-id="cf9bf-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedgroupsource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cf9bf-135">响应</span><span class="sxs-lookup"><span data-stu-id="cf9bf-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
