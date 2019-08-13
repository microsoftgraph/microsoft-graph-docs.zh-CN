---
title: 删除 trustFrameworkPolicy
description: 此操作将从 Azure AD B2C 租户中删除现有的 trustFrameworkPolicy 对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ba7ba97b18567a7fc696edba20ba743b56c6de76
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362550"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="22b39-103">删除 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="22b39-103">Delete trustFrameworkPolicy</span></span>

> <span data-ttu-id="22b39-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="22b39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22b39-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="22b39-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22b39-106">删除现有的[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="22b39-106">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="22b39-107">权限</span><span class="sxs-lookup"><span data-stu-id="22b39-107">Permissions</span></span>

<span data-ttu-id="22b39-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="22b39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="22b39-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="22b39-110">Permission type</span></span>      | <span data-ttu-id="22b39-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22b39-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22b39-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22b39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22b39-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="22b39-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="22b39-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22b39-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="22b39-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="22b39-115">Not supported.</span></span>|
|<span data-ttu-id="22b39-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="22b39-116">Application</span></span>|<span data-ttu-id="22b39-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="22b39-117">Not supported.</span></span>|

<span data-ttu-id="22b39-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="22b39-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="22b39-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22b39-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="22b39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="22b39-120">Request headers</span></span>

|<span data-ttu-id="22b39-121">名称</span><span class="sxs-lookup"><span data-stu-id="22b39-121">Name</span></span>|<span data-ttu-id="22b39-122">说明</span><span class="sxs-lookup"><span data-stu-id="22b39-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="22b39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22b39-123">Authorization</span></span>|<span data-ttu-id="22b39-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22b39-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22b39-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="22b39-126">Request body</span></span>

<span data-ttu-id="22b39-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22b39-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22b39-128">响应</span><span class="sxs-lookup"><span data-stu-id="22b39-128">Response</span></span>

<span data-ttu-id="22b39-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="22b39-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="22b39-130">示例</span><span class="sxs-lookup"><span data-stu-id="22b39-130">Example</span></span>

<span data-ttu-id="22b39-131">下面的示例删除**trustFrameworkPolicy**。</span><span class="sxs-lookup"><span data-stu-id="22b39-131">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="22b39-132">请求</span><span class="sxs-lookup"><span data-stu-id="22b39-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="22b39-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="22b39-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22b39-134">C#</span><span class="sxs-lookup"><span data-stu-id="22b39-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22b39-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22b39-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22b39-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="22b39-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="22b39-137">Java</span><span class="sxs-lookup"><span data-stu-id="22b39-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-trustframeworkpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="22b39-138">响应</span><span class="sxs-lookup"><span data-stu-id="22b39-138">Response</span></span>

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
