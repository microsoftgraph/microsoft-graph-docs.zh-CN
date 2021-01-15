---
title: 删除 identityApiConnector
description: 删除 identityApiConnector 对象。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3f021afd1285d00e71ef9ddab25210f00c8ac2be
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873680"
---
# <a name="delete-identityapiconnector"></a><span data-ttu-id="c87fc-103">删除 identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="c87fc-103">Delete identityApiConnector</span></span>

<span data-ttu-id="c87fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c87fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c87fc-105">删除 [identityApiConnector](../resources/identityapiconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c87fc-105">Deletes an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c87fc-106">权限</span><span class="sxs-lookup"><span data-stu-id="c87fc-106">Permissions</span></span>

<span data-ttu-id="c87fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c87fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c87fc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c87fc-109">Permission type</span></span>                        | <span data-ttu-id="c87fc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c87fc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c87fc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c87fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c87fc-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87fc-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="c87fc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c87fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c87fc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c87fc-114">Not supported.</span></span>  |
| <span data-ttu-id="c87fc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c87fc-115">Application</span></span>                            | <span data-ttu-id="c87fc-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87fc-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="c87fc-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="c87fc-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c87fc-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c87fc-118">Global administrator</span></span>
* <span data-ttu-id="c87fc-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="c87fc-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c87fc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c87fc-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="c87fc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c87fc-121">Request headers</span></span>
|<span data-ttu-id="c87fc-122">名称</span><span class="sxs-lookup"><span data-stu-id="c87fc-122">Name</span></span>|<span data-ttu-id="c87fc-123">说明</span><span class="sxs-lookup"><span data-stu-id="c87fc-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c87fc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c87fc-124">Authorization</span></span>|<span data-ttu-id="c87fc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c87fc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c87fc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c87fc-127">Request body</span></span>
<span data-ttu-id="c87fc-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c87fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c87fc-129">响应</span><span class="sxs-lookup"><span data-stu-id="c87fc-129">Response</span></span>

<span data-ttu-id="c87fc-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c87fc-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c87fc-131">示例</span><span class="sxs-lookup"><span data-stu-id="c87fc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c87fc-132">请求</span><span class="sxs-lookup"><span data-stu-id="c87fc-132">Request</span></span>

<span data-ttu-id="c87fc-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c87fc-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c87fc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c87fc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityapiconnector"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/apiConnectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="c87fc-135">C#</span><span class="sxs-lookup"><span data-stu-id="c87fc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c87fc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c87fc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c87fc-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c87fc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c87fc-138">Java</span><span class="sxs-lookup"><span data-stu-id="c87fc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c87fc-139">响应</span><span class="sxs-lookup"><span data-stu-id="c87fc-139">Response</span></span>

<span data-ttu-id="c87fc-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c87fc-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
