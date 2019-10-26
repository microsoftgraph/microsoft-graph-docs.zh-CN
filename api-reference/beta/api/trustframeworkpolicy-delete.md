---
title: 删除 trustFrameworkPolicy
description: 此操作将从 Azure AD B2C 租户中删除现有的 trustFrameworkPolicy 对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 77363aa262314b8d6a6d7ff3470327569159e1e7
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734421"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="f91ca-103">删除 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="f91ca-103">Delete trustFrameworkPolicy</span></span>

> <span data-ttu-id="f91ca-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f91ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f91ca-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f91ca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f91ca-106">删除现有的[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="f91ca-106">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f91ca-107">权限</span><span class="sxs-lookup"><span data-stu-id="f91ca-107">Permissions</span></span>

<span data-ttu-id="f91ca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f91ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f91ca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f91ca-110">Permission type</span></span>      | <span data-ttu-id="f91ca-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f91ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f91ca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f91ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f91ca-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="f91ca-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="f91ca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f91ca-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f91ca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f91ca-115">Not supported.</span></span>|
|<span data-ttu-id="f91ca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f91ca-116">Application</span></span>|<span data-ttu-id="f91ca-117">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="f91ca-117">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="f91ca-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="f91ca-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f91ca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f91ca-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f91ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f91ca-120">Request headers</span></span>

|<span data-ttu-id="f91ca-121">名称</span><span class="sxs-lookup"><span data-stu-id="f91ca-121">Name</span></span>|<span data-ttu-id="f91ca-122">说明</span><span class="sxs-lookup"><span data-stu-id="f91ca-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f91ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f91ca-123">Authorization</span></span>|<span data-ttu-id="f91ca-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f91ca-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f91ca-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f91ca-126">Request body</span></span>

<span data-ttu-id="f91ca-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f91ca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f91ca-128">响应</span><span class="sxs-lookup"><span data-stu-id="f91ca-128">Response</span></span>

<span data-ttu-id="f91ca-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f91ca-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f91ca-130">示例</span><span class="sxs-lookup"><span data-stu-id="f91ca-130">Example</span></span>

<span data-ttu-id="f91ca-131">下面的示例删除**trustFrameworkPolicy**。</span><span class="sxs-lookup"><span data-stu-id="f91ca-131">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="f91ca-132">请求</span><span class="sxs-lookup"><span data-stu-id="f91ca-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f91ca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f91ca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f91ca-134">C#</span><span class="sxs-lookup"><span data-stu-id="f91ca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f91ca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f91ca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f91ca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f91ca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f91ca-137">响应</span><span class="sxs-lookup"><span data-stu-id="f91ca-137">Response</span></span>

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
