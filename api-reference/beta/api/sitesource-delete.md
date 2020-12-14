---
title: 删除 siteSource
description: 删除 siteSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c4732e101fe86fdd9cafbad658bf1e3211283514
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659565"
---
# <a name="delete-sitesource"></a><span data-ttu-id="add7a-103">删除 siteSource</span><span class="sxs-lookup"><span data-stu-id="add7a-103">Delete siteSource</span></span>

<span data-ttu-id="add7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="add7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="add7a-105">删除 [siteSource](../resources/sitesource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="add7a-105">Delete a [siteSource](../resources/sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="add7a-106">权限</span><span class="sxs-lookup"><span data-stu-id="add7a-106">Permissions</span></span>

<span data-ttu-id="add7a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="add7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="add7a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="add7a-109">Permission type</span></span>|<span data-ttu-id="add7a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="add7a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="add7a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="add7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="add7a-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="add7a-112">User.Read</span></span>|
|<span data-ttu-id="add7a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="add7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="add7a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="add7a-114">Not supported.</span></span>|
|<span data-ttu-id="add7a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="add7a-115">Application</span></span>|<span data-ttu-id="add7a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="add7a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="add7a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="add7a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources/{siteSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="add7a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="add7a-118">Request headers</span></span>

|<span data-ttu-id="add7a-119">名称</span><span class="sxs-lookup"><span data-stu-id="add7a-119">Name</span></span>|<span data-ttu-id="add7a-120">说明</span><span class="sxs-lookup"><span data-stu-id="add7a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="add7a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="add7a-121">Authorization</span></span>|<span data-ttu-id="add7a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="add7a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="add7a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="add7a-124">Request body</span></span>

<span data-ttu-id="add7a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="add7a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="add7a-126">响应</span><span class="sxs-lookup"><span data-stu-id="add7a-126">Response</span></span>

<span data-ttu-id="add7a-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="add7a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="add7a-128">示例</span><span class="sxs-lookup"><span data-stu-id="add7a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="add7a-129">请求</span><span class="sxs-lookup"><span data-stu-id="add7a-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="add7a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="add7a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sitesource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources/38304445-3741-3333-4233-344238454333
```
# <a name="c"></a>[<span data-ttu-id="add7a-131">C#</span><span class="sxs-lookup"><span data-stu-id="add7a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sitesource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="add7a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="add7a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sitesource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="add7a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="add7a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sitesource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="add7a-134">Java</span><span class="sxs-lookup"><span data-stu-id="add7a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-sitesource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="add7a-135">响应</span><span class="sxs-lookup"><span data-stu-id="add7a-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
