---
title: 更新 identityProvider
description: 更新现有 identityProvider 中的属性。
localization_priority: Normal
ms.openlocfilehash: ebe49fb562f77004edfa3504130fbf50f4d40003
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832807"
---
# <a name="update-identityprovider"></a><span data-ttu-id="cbd0c-103">更新 identityProvider</span><span class="sxs-lookup"><span data-stu-id="cbd0c-103">Update identityProvider</span></span>

> <span data-ttu-id="cbd0c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbd0c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cbd0c-106">更新现有[identityProvider](../resources/identityprovider.md)中的属性。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-106">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cbd0c-107">权限</span><span class="sxs-lookup"><span data-stu-id="cbd0c-107">Permissions</span></span>

<span data-ttu-id="cbd0c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbd0c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbd0c-110">Permission type</span></span>      | <span data-ttu-id="cbd0c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cbd0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbd0c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbd0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbd0c-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbd0c-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="cbd0c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbd0c-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="cbd0c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-115">Not supported.</span></span>|
|<span data-ttu-id="cbd0c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbd0c-116">Application</span></span>|<span data-ttu-id="cbd0c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-117">Not supported.</span></span>|

<span data-ttu-id="cbd0c-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="cbd0c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbd0c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cbd0c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbd0c-120">Request headers</span></span>

|<span data-ttu-id="cbd0c-121">名称</span><span class="sxs-lookup"><span data-stu-id="cbd0c-121">Name</span></span>|<span data-ttu-id="cbd0c-122">说明</span><span class="sxs-lookup"><span data-stu-id="cbd0c-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="cbd0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbd0c-123">Authorization</span></span>|<span data-ttu-id="cbd0c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cbd0c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cbd0c-126">Content-Type</span></span>|<span data-ttu-id="cbd0c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cbd0c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbd0c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbd0c-129">Request body</span></span>

<span data-ttu-id="cbd0c-130">在请求正文中，将一个 JSON 对象，提供需要更新的一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-130">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="cbd0c-131">属性</span><span class="sxs-lookup"><span data-stu-id="cbd0c-131">Property</span></span>|<span data-ttu-id="cbd0c-132">类型</span><span class="sxs-lookup"><span data-stu-id="cbd0c-132">Type</span></span>|<span data-ttu-id="cbd0c-133">Description</span><span class="sxs-lookup"><span data-stu-id="cbd0c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbd0c-134">clientId</span><span class="sxs-lookup"><span data-stu-id="cbd0c-134">clientId</span></span>|<span data-ttu-id="cbd0c-135">字符串</span><span class="sxs-lookup"><span data-stu-id="cbd0c-135">String</span></span>|<span data-ttu-id="cbd0c-136">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-136">The client ID for the application.</span></span> <span data-ttu-id="cbd0c-137">这是注册的标识提供程序的应用程序时所获得的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="cbd0c-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="cbd0c-138">clientSecret</span></span>|<span data-ttu-id="cbd0c-139">字符串</span><span class="sxs-lookup"><span data-stu-id="cbd0c-139">String</span></span>|<span data-ttu-id="cbd0c-140">应用程序客户端机密。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-140">The client secret for the application.</span></span> <span data-ttu-id="cbd0c-141">这是注册的标识提供程序的应用程序时所获得的客户端机密。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="cbd0c-142">name</span><span class="sxs-lookup"><span data-stu-id="cbd0c-142">name</span></span>|<span data-ttu-id="cbd0c-143">字符串</span><span class="sxs-lookup"><span data-stu-id="cbd0c-143">String</span></span>|<span data-ttu-id="cbd0c-144">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-144">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="cbd0c-145">响应</span><span class="sxs-lookup"><span data-stu-id="cbd0c-145">Response</span></span>

<span data-ttu-id="cbd0c-146">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-146">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="cbd0c-147">如果不成功，`4xx`与特定的详细信息，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-147">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="cbd0c-148">示例</span><span class="sxs-lookup"><span data-stu-id="cbd0c-148">Example</span></span>

<span data-ttu-id="cbd0c-149">以下示例更新的令牌生存期**identityProvider**定义，并将其设置为默认组织。</span><span class="sxs-lookup"><span data-stu-id="cbd0c-149">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="cbd0c-150">请求</span><span class="sxs-lookup"><span data-stu-id="cbd0c-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```

##### <a name="response"></a><span data-ttu-id="cbd0c-151">响应</span><span class="sxs-lookup"><span data-stu-id="cbd0c-151">Response</span></span>

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
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
