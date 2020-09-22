---
title: 删除 identityProvider
description: 删除现有的 identityProvider
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7765b69536699e969fb721cc3dc7e65ff313ce77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973202"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="3047e-103">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="3047e-103">Delete identityProvider</span></span>

<span data-ttu-id="3047e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3047e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3047e-105">删除现有的 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="3047e-105">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3047e-106">权限</span><span class="sxs-lookup"><span data-stu-id="3047e-106">Permissions</span></span>

<span data-ttu-id="3047e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3047e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3047e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3047e-109">Permission type</span></span>      | <span data-ttu-id="3047e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3047e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3047e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3047e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3047e-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3047e-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="3047e-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="3047e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3047e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3047e-114">Not supported.</span></span>|
|<span data-ttu-id="3047e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3047e-115">Application</span></span>|<span data-ttu-id="3047e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3047e-116">Not supported.</span></span>|

<span data-ttu-id="3047e-117">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="3047e-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="3047e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3047e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3047e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3047e-119">Request headers</span></span>

|<span data-ttu-id="3047e-120">名称</span><span class="sxs-lookup"><span data-stu-id="3047e-120">Name</span></span>|<span data-ttu-id="3047e-121">说明</span><span class="sxs-lookup"><span data-stu-id="3047e-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3047e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3047e-122">Authorization</span></span>|<span data-ttu-id="3047e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3047e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3047e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3047e-125">Request body</span></span>

<span data-ttu-id="3047e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3047e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3047e-127">响应</span><span class="sxs-lookup"><span data-stu-id="3047e-127">Response</span></span>

<span data-ttu-id="3047e-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3047e-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3047e-129">示例</span><span class="sxs-lookup"><span data-stu-id="3047e-129">Example</span></span>

<span data-ttu-id="3047e-130">以下示例会删除 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="3047e-130">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="3047e-131">请求</span><span class="sxs-lookup"><span data-stu-id="3047e-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3047e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3047e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```
# <a name="c"></a>[<span data-ttu-id="3047e-133">C#</span><span class="sxs-lookup"><span data-stu-id="3047e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3047e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3047e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3047e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3047e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3047e-136">Java</span><span class="sxs-lookup"><span data-stu-id="3047e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3047e-137">响应</span><span class="sxs-lookup"><span data-stu-id="3047e-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

