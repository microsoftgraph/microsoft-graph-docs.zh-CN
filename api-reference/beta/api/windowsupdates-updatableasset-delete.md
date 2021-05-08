---
title: 删除 updatableAsset
description: 删除 updatableAsset 对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 7e266a24fd23858f60326e14b956cdf5ef731315
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240723"
---
# <a name="delete-updatableasset"></a><span data-ttu-id="0a58c-103">删除 updatableAsset</span><span class="sxs-lookup"><span data-stu-id="0a58c-103">Delete updatableAsset</span></span>
<span data-ttu-id="0a58c-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="0a58c-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a58c-105">删除 [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a58c-105">Delete an [updatableAsset](../resources/windowsupdates-updatableasset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a58c-106">权限</span><span class="sxs-lookup"><span data-stu-id="0a58c-106">Permissions</span></span>
<span data-ttu-id="0a58c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a58c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a58c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a58c-109">Permission type</span></span>|<span data-ttu-id="0a58c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a58c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a58c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a58c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a58c-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a58c-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="0a58c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a58c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a58c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a58c-114">Not supported.</span></span>|
|<span data-ttu-id="0a58c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a58c-115">Application</span></span>|<span data-ttu-id="0a58c-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a58c-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a58c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a58c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{updatableAssetId}
```

## <a name="request-headers"></a><span data-ttu-id="0a58c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a58c-118">Request headers</span></span>
|<span data-ttu-id="0a58c-119">名称</span><span class="sxs-lookup"><span data-stu-id="0a58c-119">Name</span></span>|<span data-ttu-id="0a58c-120">说明</span><span class="sxs-lookup"><span data-stu-id="0a58c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0a58c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a58c-121">Authorization</span></span>|<span data-ttu-id="0a58c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a58c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a58c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a58c-124">Request body</span></span>
<span data-ttu-id="0a58c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a58c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a58c-126">响应</span><span class="sxs-lookup"><span data-stu-id="0a58c-126">Response</span></span>

<span data-ttu-id="0a58c-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0a58c-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a58c-129">示例</span><span class="sxs-lookup"><span data-stu-id="0a58c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a58c-130">请求</span><span class="sxs-lookup"><span data-stu-id="0a58c-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0a58c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a58c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_updatableasset"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetId}
```
# <a name="c"></a>[<span data-ttu-id="0a58c-132">C#</span><span class="sxs-lookup"><span data-stu-id="0a58c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a58c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a58c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a58c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a58c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a58c-135">Java</span><span class="sxs-lookup"><span data-stu-id="0a58c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a58c-136">响应</span><span class="sxs-lookup"><span data-stu-id="0a58c-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

