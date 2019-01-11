---
title: 删除 identityProvider
description: 删除现有 identityProvider。
localization_priority: Normal
ms.openlocfilehash: 35689037d4f6a564ee3e1e40d18401ef793ef474
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808293"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="66d06-103">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="66d06-103">Delete identityProvider</span></span>

> <span data-ttu-id="66d06-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="66d06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66d06-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="66d06-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66d06-106">删除现有[identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="66d06-106">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="66d06-107">权限</span><span class="sxs-lookup"><span data-stu-id="66d06-107">Permissions</span></span>

<span data-ttu-id="66d06-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66d06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66d06-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="66d06-110">Permission type</span></span>      | <span data-ttu-id="66d06-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66d06-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66d06-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66d06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66d06-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d06-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="66d06-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66d06-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="66d06-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="66d06-115">Not supported.</span></span>|
|<span data-ttu-id="66d06-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="66d06-116">Application</span></span>|<span data-ttu-id="66d06-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="66d06-117">Not supported.</span></span>|

<span data-ttu-id="66d06-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="66d06-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="66d06-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66d06-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="66d06-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66d06-120">Request headers</span></span>

|<span data-ttu-id="66d06-121">名称</span><span class="sxs-lookup"><span data-stu-id="66d06-121">Name</span></span>|<span data-ttu-id="66d06-122">说明</span><span class="sxs-lookup"><span data-stu-id="66d06-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="66d06-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66d06-123">Authorization</span></span>|<span data-ttu-id="66d06-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66d06-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66d06-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="66d06-126">Request body</span></span>

<span data-ttu-id="66d06-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66d06-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66d06-128">响应</span><span class="sxs-lookup"><span data-stu-id="66d06-128">Response</span></span>

<span data-ttu-id="66d06-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="66d06-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="66d06-130">示例</span><span class="sxs-lookup"><span data-stu-id="66d06-130">Example</span></span>

<span data-ttu-id="66d06-131">下面的示例删除**identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="66d06-131">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="66d06-132">请求</span><span class="sxs-lookup"><span data-stu-id="66d06-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="66d06-133">响应</span><span class="sxs-lookup"><span data-stu-id="66d06-133">Response</span></span>

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
  "tocPath": ""
}-->
