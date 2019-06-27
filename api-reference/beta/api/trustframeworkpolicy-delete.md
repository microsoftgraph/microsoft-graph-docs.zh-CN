---
title: 删除 trustFrameworkPolicy
description: 此操作将从 Azure AD B2C 租户中删除现有的 trustFrameworkPolicy 对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f1e716c854b0dfdd387b56e5fa60646725010dc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270531"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="a9677-103">删除 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="a9677-103">Delete trustFrameworkPolicy</span></span>

> <span data-ttu-id="a9677-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a9677-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9677-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a9677-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9677-106">删除现有的[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="a9677-106">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9677-107">权限</span><span class="sxs-lookup"><span data-stu-id="a9677-107">Permissions</span></span>

<span data-ttu-id="a9677-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a9677-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="a9677-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9677-110">Permission type</span></span>      | <span data-ttu-id="a9677-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9677-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9677-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9677-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9677-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="a9677-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="a9677-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9677-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a9677-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9677-115">Not supported.</span></span>|
|<span data-ttu-id="a9677-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9677-116">Application</span></span>|<span data-ttu-id="a9677-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9677-117">Not supported.</span></span>|

<span data-ttu-id="a9677-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="a9677-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="a9677-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9677-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a9677-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9677-120">Request headers</span></span>

|<span data-ttu-id="a9677-121">名称</span><span class="sxs-lookup"><span data-stu-id="a9677-121">Name</span></span>|<span data-ttu-id="a9677-122">说明</span><span class="sxs-lookup"><span data-stu-id="a9677-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a9677-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9677-123">Authorization</span></span>|<span data-ttu-id="a9677-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9677-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9677-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9677-126">Request body</span></span>

<span data-ttu-id="a9677-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9677-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9677-128">响应</span><span class="sxs-lookup"><span data-stu-id="a9677-128">Response</span></span>

<span data-ttu-id="a9677-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a9677-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9677-130">示例</span><span class="sxs-lookup"><span data-stu-id="a9677-130">Example</span></span>

<span data-ttu-id="a9677-131">下面的示例删除**trustFrameworkPolicy**。</span><span class="sxs-lookup"><span data-stu-id="a9677-131">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="a9677-132">请求</span><span class="sxs-lookup"><span data-stu-id="a9677-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```

##### <a name="response"></a><span data-ttu-id="a9677-133">响应</span><span class="sxs-lookup"><span data-stu-id="a9677-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a9677-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a9677-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a9677-135">C#</span><span class="sxs-lookup"><span data-stu-id="a9677-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_trustFrameworkPolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9677-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="a9677-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_trustFrameworkPolicy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a9677-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="a9677-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_trustFrameworkPolicy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/trustframeworkpolicy-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/trustframeworkpolicy-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/trustframeworkpolicy-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
