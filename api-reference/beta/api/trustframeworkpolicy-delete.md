---
title: 删除 trustFrameworkPolicy
description: 此操作从 Azure AD B2C 租户中删除现有 trustFrameworkPolicy 对象。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0ebca87f50af1d4db6c4b6053bcabcaf9aa672d3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444950"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="a8d17-103">删除 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="a8d17-103">Delete trustFrameworkPolicy</span></span>

<span data-ttu-id="a8d17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8d17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8d17-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a8d17-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8d17-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8d17-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8d17-107">删除现有的 [trustFrameworkPolicy](../resources/trustframeworkpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="a8d17-107">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8d17-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="a8d17-108">Permissions</span></span>

<span data-ttu-id="a8d17-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a8d17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="a8d17-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8d17-111">Permission type</span></span>      | <span data-ttu-id="a8d17-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8d17-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8d17-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8d17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8d17-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="a8d17-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="a8d17-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8d17-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a8d17-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8d17-116">Not supported.</span></span>|
|<span data-ttu-id="a8d17-117">Application</span><span class="sxs-lookup"><span data-stu-id="a8d17-117">Application</span></span>|<span data-ttu-id="a8d17-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="a8d17-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="a8d17-119">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="a8d17-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="a8d17-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8d17-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a8d17-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8d17-121">Request headers</span></span>

|<span data-ttu-id="a8d17-122">名称</span><span class="sxs-lookup"><span data-stu-id="a8d17-122">Name</span></span>|<span data-ttu-id="a8d17-123">说明</span><span class="sxs-lookup"><span data-stu-id="a8d17-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a8d17-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8d17-124">Authorization</span></span>|<span data-ttu-id="a8d17-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8d17-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8d17-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8d17-127">Request body</span></span>

<span data-ttu-id="a8d17-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a8d17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8d17-129">响应</span><span class="sxs-lookup"><span data-stu-id="a8d17-129">Response</span></span>

<span data-ttu-id="a8d17-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a8d17-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a8d17-131">示例</span><span class="sxs-lookup"><span data-stu-id="a8d17-131">Example</span></span>

<span data-ttu-id="a8d17-132">下面的示例删除 **trustFrameworkPolicy**。</span><span class="sxs-lookup"><span data-stu-id="a8d17-132">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="a8d17-133">请求</span><span class="sxs-lookup"><span data-stu-id="a8d17-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a8d17-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8d17-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```
# <a name="c"></a>[<span data-ttu-id="a8d17-135">C#</span><span class="sxs-lookup"><span data-stu-id="a8d17-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8d17-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8d17-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8d17-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8d17-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8d17-138">Java</span><span class="sxs-lookup"><span data-stu-id="a8d17-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-trustframeworkpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a8d17-139">响应</span><span class="sxs-lookup"><span data-stu-id="a8d17-139">Response</span></span>

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
  "description": "Delete trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


