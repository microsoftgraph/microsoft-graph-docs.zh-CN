---
title: 删除部署
description: 删除部署对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 3baf7f9d163c7f1f4beb8967ca8cb94b53fb95f5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241375"
---
# <a name="delete-deployment"></a><span data-ttu-id="8abd7-103">删除部署</span><span class="sxs-lookup"><span data-stu-id="8abd7-103">Delete deployment</span></span>
<span data-ttu-id="8abd7-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="8abd7-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8abd7-105">删除 [部署](../resources/windowsupdates-deployment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8abd7-105">Delete a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8abd7-106">权限</span><span class="sxs-lookup"><span data-stu-id="8abd7-106">Permissions</span></span>
<span data-ttu-id="8abd7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8abd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8abd7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8abd7-109">Permission type</span></span>|<span data-ttu-id="8abd7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8abd7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8abd7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8abd7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8abd7-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abd7-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="8abd7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8abd7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8abd7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8abd7-114">Not supported.</span></span>|
|<span data-ttu-id="8abd7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8abd7-115">Application</span></span>|<span data-ttu-id="8abd7-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abd7-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8abd7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8abd7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/deployments/{deploymentId}
```

## <a name="request-headers"></a><span data-ttu-id="8abd7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8abd7-118">Request headers</span></span>
|<span data-ttu-id="8abd7-119">名称</span><span class="sxs-lookup"><span data-stu-id="8abd7-119">Name</span></span>|<span data-ttu-id="8abd7-120">说明</span><span class="sxs-lookup"><span data-stu-id="8abd7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8abd7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8abd7-121">Authorization</span></span>|<span data-ttu-id="8abd7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8abd7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8abd7-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8abd7-124">Request body</span></span>
<span data-ttu-id="8abd7-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8abd7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8abd7-126">响应</span><span class="sxs-lookup"><span data-stu-id="8abd7-126">Response</span></span>

<span data-ttu-id="8abd7-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8abd7-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8abd7-129">示例</span><span class="sxs-lookup"><span data-stu-id="8abd7-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8abd7-130">请求</span><span class="sxs-lookup"><span data-stu-id="8abd7-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8abd7-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8abd7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_deployment"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}
```
# <a name="c"></a>[<span data-ttu-id="8abd7-132">C#</span><span class="sxs-lookup"><span data-stu-id="8abd7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-deployment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8abd7-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8abd7-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-deployment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8abd7-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8abd7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-deployment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8abd7-135">Java</span><span class="sxs-lookup"><span data-stu-id="8abd7-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-deployment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8abd7-136">响应</span><span class="sxs-lookup"><span data-stu-id="8abd7-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

