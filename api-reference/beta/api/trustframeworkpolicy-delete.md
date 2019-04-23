---
title: 删除 trustFrameworkPolicy
description: 此操作将从 Azure AD B2C 租户中删除现有的 trustFrameworkPolicy 对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2583cbf5fd8feee12b18482c515490d2de8ce8be
ms.sourcegitcommit: d264fa064215879fa88a4680402cd57a470d73db
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2019
ms.locfileid: "31989399"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="ca377-103">删除 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="ca377-103">Delete trustFrameworkPolicy</span></span>

> <span data-ttu-id="ca377-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca377-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca377-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca377-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca377-106">删除现有的[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="ca377-106">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca377-107">权限</span><span class="sxs-lookup"><span data-stu-id="ca377-107">Permissions</span></span>

<span data-ttu-id="ca377-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ca377-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="ca377-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca377-110">Permission type</span></span>      | <span data-ttu-id="ca377-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca377-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca377-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca377-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca377-113">TrustFramework</span><span class="sxs-lookup"><span data-stu-id="ca377-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="ca377-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca377-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ca377-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca377-115">Not supported.</span></span>|
|<span data-ttu-id="ca377-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca377-116">Application</span></span>|<span data-ttu-id="ca377-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca377-117">Not supported.</span></span>|

<span data-ttu-id="ca377-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="ca377-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="ca377-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca377-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ca377-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca377-120">Request headers</span></span>

|<span data-ttu-id="ca377-121">名称</span><span class="sxs-lookup"><span data-stu-id="ca377-121">Name</span></span>|<span data-ttu-id="ca377-122">说明</span><span class="sxs-lookup"><span data-stu-id="ca377-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ca377-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca377-123">Authorization</span></span>|<span data-ttu-id="ca377-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca377-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca377-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca377-126">Request body</span></span>

<span data-ttu-id="ca377-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca377-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca377-128">响应</span><span class="sxs-lookup"><span data-stu-id="ca377-128">Response</span></span>

<span data-ttu-id="ca377-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ca377-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ca377-130">示例</span><span class="sxs-lookup"><span data-stu-id="ca377-130">Example</span></span>

<span data-ttu-id="ca377-131">下面的示例删除**trustFrameworkPolicy**。</span><span class="sxs-lookup"><span data-stu-id="ca377-131">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="ca377-132">请求</span><span class="sxs-lookup"><span data-stu-id="ca377-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```

##### <a name="response"></a><span data-ttu-id="ca377-133">响应</span><span class="sxs-lookup"><span data-stu-id="ca377-133">Response</span></span>

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
  "tocPath": ""
}-->
