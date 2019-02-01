---
title: 删除 identityProvider
description: 删除现有的 identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a09018011e87da383371ba41b1a046ddeb9002b5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649371"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="e7884-103">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="e7884-103">Delete identityProvider</span></span>

<span data-ttu-id="e7884-104">删除现有的 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="e7884-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7884-105">权限</span><span class="sxs-lookup"><span data-stu-id="e7884-105">Permissions</span></span>

<span data-ttu-id="e7884-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7884-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7884-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7884-108">Permission type</span></span>      | <span data-ttu-id="e7884-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7884-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7884-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7884-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e7884-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7884-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e7884-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="e7884-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e7884-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7884-113">Not supported.</span></span>|
|<span data-ttu-id="e7884-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7884-114">Application</span></span>|<span data-ttu-id="e7884-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7884-115">Not supported.</span></span>|

<span data-ttu-id="e7884-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="e7884-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e7884-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7884-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e7884-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7884-118">Request headers</span></span>

|<span data-ttu-id="e7884-119">名称</span><span class="sxs-lookup"><span data-stu-id="e7884-119">Name</span></span>|<span data-ttu-id="e7884-120">说明</span><span class="sxs-lookup"><span data-stu-id="e7884-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e7884-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7884-121">Authorization</span></span>|<span data-ttu-id="e7884-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e7884-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7884-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7884-124">Request body</span></span>

<span data-ttu-id="e7884-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e7884-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7884-126">响应</span><span class="sxs-lookup"><span data-stu-id="e7884-126">Response</span></span>

<span data-ttu-id="e7884-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e7884-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e7884-128">示例</span><span class="sxs-lookup"><span data-stu-id="e7884-128">Example</span></span>

<span data-ttu-id="e7884-129">以下示例会删除 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="e7884-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e7884-130">请求</span><span class="sxs-lookup"><span data-stu-id="e7884-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="e7884-131">响应</span><span class="sxs-lookup"><span data-stu-id="e7884-131">Response</span></span>

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
